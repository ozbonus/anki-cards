---
description: "Enforces TSV formatting rules for Anki flashcard output files"
applyTo: "output.tsv"
---

When editing or generating `output.tsv`:

- The file must be tab-separated with exactly six columns per row.
- The header row is: `English\tEnglish_context\t台灣國語\t台灣國語_context\t日本語\t日本語_context`
- Every Chinese character in 台灣國語 and 台灣國語_context fields must have Zhuyin (注音) in brackets immediately after it — e.g., `書[ㄕㄨ]`.
- Every Kanji or Kanji compound in 日本語 and 日本語_context fields must have Hiragana furigana in brackets — e.g., `猫[ねこ]`.
- Use full-width punctuation in Mandarin and Japanese fields (。，！？、：；).
- Do not quote fields. Fields must not contain literal tabs or newlines.
- Excluded language columns must be empty strings (consecutive tabs), not omitted.
