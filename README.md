# ML Builds

Pre-built shared libraries for machine learning

Library | Linux x86 | ARM | Mac x86 | ARM | Windows | Files | License
--- | --- | --- | --- | --- | --- | --- | ---
[Bling Fire](https://github.com/Microsoft/BlingFire) | ✓ | ✓ | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/blingfire-0.1.3) | MIT
[cmfrec](https://github.com/david-cortes/cmfrec) | ✓ | | ✓ | ✓ | | [View](https://github.com/ankane/ml-builds/releases/tag/cmfrec-2.4.1) | MIT
[Faiss](https://github.com/facebookresearch/faiss) | ✓ | | ✓ | | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/faiss-1.6.1) | MIT
[Interpret](https://github.com/interpretml/interpret) | ✓ | | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/interpret-0.2.2) | MIT
[LIBMF](https://github.com/cjlin1/libmf) | ✓ | ✓ | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/libmf-master-2) | BSD-3-Clause
[MITIE](https://github.com/mit-nlp/MITIE) | ✓ | | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/mitie-0.7) | BSL-1.0
[Multicore t-SNE](https://github.com/DmitryUlyanov/Multicore-TSNE) | ✓ | | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/multicore-tsne-master) | BSD-3-Clause
[NGT](https://github.com/yahoojapan/NGT) | ✓ | ✓ | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/ngt-1.12.2) | Apache-2.0
[SCS](https://github.com/cvxgrp/scs) | ✓ | | ✓ | | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/scs-2.0.2) | MIT
[ThunderSVM](https://github.com/Xtra-Computing/thundersvm) | ✓ | | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/thundersvm-0.3.4) | Apache-2.0
[XGBoost](https://github.com/dmlc/xgboost) | ✓ | ✓ | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xgboost-1.3.0) | Apache-2.0
[xLearn](https://github.com/aksnzhy/xlearn) | ✓ | n/a | ✓ | n/a | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xlearn-0.4.4) | Apache-2.0
[Argon2](https://github.com/P-H-C/phc-winner-argon2) (non-ML) | ✓ | ✓ | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/argon2-20190702) | CC0-1.0

Notes

- LIBMF: Fork, no OpenMP
- Multicore t-SNE: Fork with OpenMP for Mac x86
- SCS: No blas/lapack on Windows
- XGBoost: No OpenMP on Windows

View the [build scripts](.github/workflows)

Some projects include shared libraries as part of their releases:

- [LibTorch](https://pytorch.org/)
- [LightGBM](https://github.com/microsoft/LightGBM/releases)
- [ONNX Runtime](https://github.com/microsoft/onnxruntime/releases)
- [OR-Tools](https://developers.google.com/optimization/install/cpp)
- [OSQP](https://bintray.com/bstellato/generic/OSQP#files)

Library | Linux ARM | Mac ARM | Files | License
--- | --- | --- | --- | ---
[LightGBM](https://github.com/Microsoft/LightGBM) | | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/lightgbm-3.1.1) | MIT
[OSQP](https://github.com/oxfordcontrol/osqp) | | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/osqp-0.6.2) | Apache-2.0

## Details

For portability:

- Linux x86 libraries are built with `-march=x86-64` (when possible) and older `glibc` (todo: build with much older)
- Linux ARM libraries are built with `-march=armv8-a` (when possible) and older `glibc` (todo: build with much older)
- Mac x86 libraries are built with `-march=nehalem` (same as Homebrew) and `MACOSX_DEPLOYMENT_TARGET=10.13`
- Mac ARM libraries are built with `-march=armv8-a` and `MACOSX_DEPLOYMENT_TARGET=11.0`

References:

- [x86](https://gcc.gnu.org/onlinedocs/gcc/x86-Options.html)
- [ARM](https://gcc.gnu.org/onlinedocs/gcc/ARM-Options.html)

Other notes:

- Windows libraries are built with `-A x64`
- Mac libraries that use OpenMP require `brew install libomp` (Faiss, Multicore t-SNE, NGT, ThunderSVM, XGBoost)
