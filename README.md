# ML Builds

Pre-built shared libraries for machine learning

Library | Linux | Mac | Windows | Assets | Notes
--- | --- | --- | --- | --- | ---
BlingFire | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/blingfire-master) |
Faiss | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/faiss-1.6.1) |
Interpret | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/interpret-master) | |
LIBMF | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/libmf-master) | Fork, OpenMP disabled
Multicore t-SNE | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/multicore-tsne-master) |
NGT | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/ngt-1.10.0) |
SCS | ✓ | ✓ | | [View](https://github.com/ankane/ml-builds/releases/tag/scs-2.0.2) |
ThunderSVM | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/thundersvm-0.3.4) |
XGBoost | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xgboost-1.0.2) | OpenMP disabled (Windows)
xLearn | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xlearn-0.4.4) |

View the [build scripts](.github/workflows)

Some projects include shared libraries as part of their releases:

- [LightGBM](https://github.com/microsoft/LightGBM/releases)
- [LibTorch](https://pytorch.org/)
- [ONNX Runtime](https://github.com/microsoft/onnxruntime/releases)
- [OR-Tools](https://developers.google.com/optimization/install/cpp)
- [OSQP](https://bintray.com/bstellato/generic/OSQP#files)

## Details

For portability:

- Linux libraries are built with older `glibc` (todo: build with much older) and `-march=x86-64` (when possible)
- Mac libraries are built with `-march=nehalem` (same as Homebrew) and `MACOSX_DEPLOYMENT_TARGET=10.13`

[Reference](https://gcc.gnu.org/onlinedocs/gcc/x86-Options.html)
