## jpegli
[![Status](https://github.com/gen2brain/jpegli/actions/workflows/test.yml/badge.svg)](https://github.com/gen2brain/jpegli/actions)
[![Go Reference](https://pkg.go.dev/badge/github.com/gen2brain/jpegli.svg)](https://pkg.go.dev/github.com/gen2brain/jpegli)

Go encoder/decoder for [JPEG](https://en.wikipedia.org/wiki/JPEG).

Based on [jpegli](https://github.com/google/jpegli) from libjxl compiled to [WASM](https://en.wikipedia.org/wiki/WebAssembly) and used with [wazero](https://wazero.io/) runtime (CGo-free).

For a pure Go alternative, see [jpegn](https://github.com/gen2brain/jpegn), a JPEG decoder and encoder with jpegli's adaptive quantization, SIMD support, no CGo/WASM and no dependencies.

### Build tags

* `wasm2go` - transpile the WASM to pure Go with [wasm2go](https://github.com/ncruces/wasm2go) instead of running it with wazero

On `arm64` the `wasm2go` backend is always used.

### Resources

* https://giannirosato.com/blog/post/jpegli/
* https://cloudinary.com/blog/jpeg-xl-and-the-pareto-front
* https://github.com/google-research/google-research/tree/master/mucped23
