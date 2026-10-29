# Halloween Jumpscare assets

Public downloads for the Halloween Jumpscare app. The app itself is not in
this repository.

## Speech model (model-v1)

Release [`model-v1`](https://github.com/phakpin/halloween-jumpscare-assets/releases/tag/model-v1) holds
the English speech recognition model used by the app's keyword mode
(`zipformer-en-20M-2023-02-17-int8-v1`). The app downloads these files once and checks their size and
SHA-256 before using them:

| File | Bytes | SHA-256 |
|---|---|---|
| `encoder-epoch-99-avg-1.int8.onnx` | 42845182 | `3810755ce7c3ab26b42a8bcf39d191308fa27fb0f53358823ba46141d03b7eb3` |
| `decoder-epoch-99-avg-1.int8.onnx` | 539499 | `21e2a2acd961b3ac72f55be2f10f1a285e1b0b0ba010d7c0b6eab141411b163c` |
| `joiner-epoch-99-avg-1.int8.onnx` | 259572 | `e085d73b593cf9b0707f370dbd656d58327d3fe36d80d849202ef81df02cb01e` |
| `tokens.txt` | 5048 | `49e3c2646595fd907228b3c6787069658f67b17377c60aeb8619c4551b2316fb` |

### Source and license

The files are an unmodified copy of
[csukuangfj/sherpa-onnx-streaming-zipformer-en-20M-2023-02-17](https://huggingface.co/csukuangfj/sherpa-onnx-streaming-zipformer-en-20M-2023-02-17) at revision
`d42f2d9f7ca24806fb667456a18a9f1b60f70d16`, by the k2-fsa / sherpa-onnx project, exported from
[desh2608/icefall-asr-librispeech-pruned-transducer-stateless7-streaming-small](https://huggingface.co/desh2608/icefall-asr-librispeech-pruned-transducer-stateless7-streaming-small).

They are licensed under the **Apache License 2.0** (see `LICENSE`). We
redistribute them without changes.
