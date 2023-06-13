![windows-ggml](https://github.com/appvoid/windows-ggml/blob/2523c4992cda97e3a5cc6d6c3221e7db811c84c1/windows-ggml.png)
### Tensor library for machine learning on Windows
This version of GGML makes it possible to build the binaries using MinGW.

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

1. Clone the repo: `git clone https://github.com/hackerexpuesto/windows-ggml.git`
1. Download [w64devkit](https://github.com/skeeto/w64devkit/releases/download/v1.19.0/w64devkit-1.19.0.zip).
2. Extract w64devkit on your pc.
3. Run w64devkit.exe.
4. Use the `cd` command to reach the windows-ggml folder.

From here you can run

```console
mkdir build && cd build
cmake -G "MinGW Makefiles" ..
make -j4 gpt-2
```
