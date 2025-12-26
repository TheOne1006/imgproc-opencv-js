# imgproc-opencv-js

Build OpenCV.js (WebAssembly) from the official OpenCV source.

## CI

The GitHub Actions workflow builds OpenCV.js and uploads the output directory as an artifact.

## Local build

Install Emscripten and make sure `emcmake` / `emmake` are available in your shell.

Then build OpenCV.js:

```bash
emcmake python3 ./opencv/platforms/js/build_js.py build_wasm --build_wasm --build_loader
```

Outputs are generated under:

```text
./opencv/build_wasm/bin/
```
