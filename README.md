# ML Builds

Pre-built shared libraries for machine learning

Library | Linux | Mac | Windows | Assets | Official | Notes
--- | --- | --- | --- | --- | --- | ---
Faiss | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/faiss-1.6.1) | |
LIBMF | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/libmf-master) | | OpenMP disabled
LightGBM | ✓ | ✓ | ✓ | [View](https://github.com/microsoft/LightGBM/releases) | ✓ |
Multicore t-SNE | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/multicore-tsne-master) | |
NGT | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/ngt-1.8.4) | |
ONNX Runtime | ✓ | ✓ | ✓ | [View](https://github.com/microsoft/onnxruntime/releases) | ✓ |
OSQP | ✓ | ✓ | ✓ | [View](https://bintray.com/bstellato/generic/OSQP#files) | ✓ |
SCS | ✓ | ✓ | | [View](https://github.com/ankane/ml-builds/releases/tag/scs-2.0.2) | |
ThunderSVM | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/thundersvm-0.3.4) | |
Vowpal Wabbit | | | | todo | | Boost dependency
XGBoost | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xgboost-0.90) | | OpenMP disabled (Mac, Windows)
xLearn | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xlearn-0.4.4) | |

View the [build scripts](.github/workflows)

## Details

For portability, shared libraries are built with:

- `-march=x86-64` on Linux (when possible)
- `-march=nehalem` on Mac (same as Homebrew)

[Reference](https://gcc.gnu.org/onlinedocs/gcc/x86-Options.html)
