# cosmo-cute-shaderc

[Offline shader compiler](https://randygaul.github.io/cute_framework/topics/shader_compilation/) for [Cute Framework](https://randygaul.github.io/cute_framework/), built with [cosmocc](https://github.com/jart/cosmopolitan).

TL;DR: Download the latest release [here](https://github.com/bullno1/cosmo-cute-shaderc/releases), it should run on your computer.

# Motivation

Building glslang is always the most time consuming part in any project powered by Cute Framework.
Moreover, in a web build, the shader has to be transpiled into GLSL ES 3.0 first.
It is not easy to build only the shader compiler as a native executable and the rest of the project as wasm.

What if the shader compiler itself can just be built once and run everywhere?
A lot of build scripts can be simplified to just: download this executable, run it.
