# ggml

Tensor library for machine learning

This version of GGML makes it possible to build the binaries on Windows devices.

## Features

- Written in C
- 16-bit float support
- 4-bit integer quantization support
- Automatic differentiation (WIP in progress)
- ADAM and L-BFGS optimizers
- Optimized for Apple silicon via NEON intrinsics and Accelerate framework
- On x86 architectures utilzes AVX intrinsics
- No third-party dependencies
- Zero memory allocations during runtime

Here is how to run the example programs:

1. Download the latest version of [w64devkit](https://github.com/skeeto/w64devkit/releases).
2. Extract w64devkit on your pc.
3. Run w64devkit.exe.
4. Use the `cd` command to reach the windows-ggml folder.

From here you can run

```console
mkdir build && cd build
cmake -G "MinGW Makefiles" ..
make -j4 gpt-2
```
