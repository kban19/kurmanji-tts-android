# Third-Party Notices

Kurmanji-TTS is proprietary software, but it bundles permissively licensed
open-source components. Those components remain under their own licences — the
MIT License and the Apache License, Version 2.0. No GPL-licensed component is
included, and the GPL-3.0 `eSpeak NG` data is not shipped: Kurmanji
grapheme-to-phoneme conversion is implemented inside the application.

The complete licence texts are also bundled inside the app under
**Settings → About → Open Source Licenses**.

| Component | Version / source | License |
| --- | --- | --- |
| Kurmancî TTS voice model | [atenax/kurmanci-tts-piper](https://huggingface.co/atenax/kurmanci-tts-piper) | MIT |
| sherpa-onnx | 2.0.1, [k2-fsa/sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) | Apache-2.0 |
| ONNX Runtime | [microsoft/onnxruntime](https://github.com/microsoft/onnxruntime) | MIT |
| AndroidX, Jetpack Compose, Room | [Android Open Source Project](https://cs.android.com/) | Apache-2.0 |
| Kotlin, kotlinx.coroutines | [JetBrains](https://github.com/JetBrains/kotlin) | Apache-2.0 |

---

## Kurmancî TTS voice model

```
Copyright (c) atenax (huggingface.co/atenax/kurmanci-tts-piper)
```

The 90-speaker Kurmanji Piper voice model (`model.onnx`, `model.onnx.json`)
by **atenax** is distributed under the **MIT License**. The model was trained
on the [atenax/kmr_tts](https://huggingface.co/datasets/atenax/kmr_tts) corpus,
which is released under **CC0-1.0**.

```
MIT License

Copyright (c) atenax

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## sherpa-onnx 2.0.1

```
Copyright 2022-2026 The sherpa-onnx authors (k2-fsa)
```

Licensed under the **Apache License, Version 2.0**. The application packages the
sherpa-onnx 2.0.1 JNI, C and C++ libraries for the four supported Android ABIs
(`arm64-v8a`, `armeabi-v7a`, `x86`, `x86_64`), with GPL-3.0 `eSpeak NG`
removed. Kurmanji grapheme-to-phoneme conversion is performed by the
application's own Hawar-alphabet phonemizer and its bundled lexicon.

## ONNX Runtime

```
Copyright (c) Microsoft Corporation
```

Licensed under the **MIT License**. ONNX Runtime is bundled inside the
sherpa-onnx archive (`libonnxruntime.so`) and performs on-device neural network
inference.

## AndroidX, Jetpack Compose and Room

```
Copyright (C) The Android Open Source Project
```

Licensed under the **Apache License, Version 2.0**. Used for the user
interface, lifecycle handling and the local recording database.

## Kotlin and kotlinx.coroutines

```
Copyright (C) 2010-2026 JetBrains s.r.o. and Kotlin contributors
```

Licensed under the **Apache License, Version 2.0**.
