---
name: typeless-link
description: Takes raw voice-transcribed text from Typeless speech recognition and transforms it into polished, usable content — notes, code, or documentation. Use when the user pastes dictated text that needs cleanup and restructuring.
argument-hint: [raw voice-transcribed text]
---

Process the following Typeless voice-transcribed input and produce clean, usable content:

$ARGUMENTS

Steps:
1. Read the raw text — it may contain speech artifacts, repetitions, or informal phrasing
2. Identify the intent: is this a concept explanation, a code request, a question, or a note?
3. Based on intent, produce one of:
   - **Learning note**: structured Markdown with key points and examples from this deep learning codebase
   - **Code snippet**: clean Python code referencing the relevant file in this repo (use Glob/Grep to find it)
   - **Documentation**: polished paragraph suitable for a README or notebook cell
4. If the content relates to a chapter or layer in this project, link to the relevant notebook under `notebooks/` or source file under `common/`
5. Output the finished content ready to paste — no explanation needed, just the result
