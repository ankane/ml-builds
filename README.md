# ML Builds

Pre-built shared libraries for machine learning

Library | Linux | Mac | Windows | Assets | Official | Notes
--- | --- | --- | --- | --- | --- | ---
BlingFire | ✓ | ✓ | ✓ | todo | |
Faiss | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/faiss-1.6.1) | |
Interpret | ✓ | ✓ | ✓ | todo | |
LIBMF | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/libmf-master) | | OpenMP disabled
LightGBM | ✓ | ✓ | ✓ | [View](https://github.com/microsoft/LightGBM/releases) | ✓ |
Multicore t-SNE | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/multicore-tsne-master) | |
NGT | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/ngt-1.8.4) | |
ONNX Runtime | ✓ | ✓ | ✓ | [View](https://github.com/microsoft/onnxruntime/releases) | ✓ |
OSQP | ✓ | ✓ | ✓ | [View](https://bintray.com/bstellato/generic/OSQP#files) | ✓ |
SCS | ✓ | ✓ | | [View](https://github.com/ankane/ml-builds/releases/tag/scs-2.0.2) | |
ThunderSVM | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/thundersvm-0.3.4) | |
Vowpal Wabbit | | | | todo | | Boost dependency
XGBoost | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xgboost-0.90) | | OpenMP disabled (Windows)
xLearn | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xlearn-0.4.4) | |

View the [build scripts](.github/workflows)

## Details

For portability:

- Linux libraries are built with older `glibc` (todo: build with much older) and `-march=x86-64` (when possible)
- Mac libraries are built with `-march=nehalem` (same as Homebrew)

[Reference](https://gcc.gnu.org/onlinedocs/gcc/x86-Options.html)
