# Paint By Relaxation
A simplified implementation of paper [Paint by relaxation](https://ieeexplore.ieee.org/document/934657), coursework for Computer Vision course at Cardiff University in 2022.

### Compile
```bash
javac Relaxation.java
```

### Usage Help
```bash
Usage:
> java Relaxation -h | --help
> java Relaxation <input_image> <compact_brush> <elongated_brush> <density> [-f] [-r <seed>] [-g <std>] [-n <std2>]
Options:
  -f force the program to proceed with an input image at any size
  -r specify a random seed for a consistent output
  -g specify a standard deviation for optional gaussian blurred versions of the output images
  -n specify a standard deviation for optional gaussian noise added to the smaller strokes in the painting
```
The `-g` option is pretty useless, but `-n` option can sometimes add a tiny bit of desired randomness.

| Input Image | Painted Output | With Imperfection (`-n 100`) |
|----------------------------------|----------------------------------|----------------------------------|
| ![sushi-cat-original](https://github.com/user-attachments/assets/03c5064d-5f02-47ad-bf00-96bd115799b4) | ![sushi-cat-painted](https://github.com/user-attachments/assets/6bf42780-cfc9-40ba-bc88-9b99f4589b50) | ![sushi-cat-painted-n-100](https://github.com/user-attachments/assets/0b2dbcfe-69ad-4712-b3c3-24f723e69deb) |
