# ML Builds

Pre-built shared libraries for machine learning

Library | Linux | Mac | Windows | Assets | Official
--- | --- | --- | --- | --- | ---
Faiss | ✓ | ✓ | n/a | todo |
LIBMF | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/libmf-201) |
LightGBM | ✓ | ✓ | ✓ | [View](https://github.com/microsoft/LightGBM/releases) | ✓
NGT | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/ngt-1.8.4) |
ONNX Runtime | ✓ | ✓ | ✓ | [View](https://github.com/microsoft/onnxruntime/releases) | ✓
OSQP | ✓ | ✓ | ✓ | [View](https://bintray.com/bstellato/generic/OSQP#files) | ✓
ThunderSVM | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/thundersvm-0.3.4) |
Vowpal Wabbit | | | | todo |
XGBoost | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xgboost-0.90) |
xLearn | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xlearn-0.4.4) |

View the [build scripts](.github/workflows)

## Details

For portability, shared libraries are built with:

- `-march=x86-64` on Linux (when possible)
- `-march=nehalem` on Mac (same as Homebrew)
