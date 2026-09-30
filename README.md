# Dictation Fast models

Speech-recognition model files downloaded by the Dictation Fast app on the user's request. No code.

## ivrit-turbo-int8 (release `ivrit-turbo-int8-2026.09.30`)

Hebrew speech recognition used by Dictation Fast when Hebrew is detected.

- Source: [ivrit-ai/whisper-large-v3-turbo](https://huggingface.co/ivrit-ai/whisper-large-v3-turbo), revision `f33172a8c3c6efbc040a7200e00835257cac0447`, by [ivrit.ai](https://www.ivrit.ai), licensed Apache-2.0.
- Change: converted to CTranslate2 format with int8 weights (`ct2-transformers-converter --quantization int8_float16`, CTranslate2 4.8.2). Nothing else was changed.
- Measured 2026-09-30 on 6 public Google FLEURS Hebrew clips: character error rate 0.102 (float16 original: 0.104).

Each file's SHA-256 is listed in the release notes, and the app checks it before use.

## License

The model files are redistributed under the Apache License 2.0 of the original work; see `LICENSE`. Copyright of the original model: ivrit.ai.
