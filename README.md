
# Hough Transform CUDA Project

This project is an implementation of the Hough Transform algorithm using CUDA. There are three main programs:

1. `houghBase`: The basic implementation of the Hough Transform.
2. `houghConst`: This version uses constant memory for storing precomputed sin and cos values.
3. `houghShared`: This version uses shared memory for storing the Hough space.

## How to Compile

The project uses a Makefile for compiling the source code. The Makefile includes targets for each version of the Hough Transform algorithm and for the utility PGM file.

Use the following command to compile all programs, we have a Makefile:

```
make
```

This will compile the source files and produce the following executables: `houghBase`, `houghConst`, and `houghShared`.

## How to Run

Once you have compiled and used 
```
make
```

The `run1`, `run2`, and `run3` commands in the Makefile run the `houghBase`, `houghConst`, and `houghShared` programs, respectively, with the `runway.pgm` image and a threshold of 4000.

For example, to run the basic version of the Hough Transform, use:
```
make run1
```

For the version that uses constant memory, use:
```
make run2
```

And for the version that uses shared memory, use:

```
make run3
```

## Notes

The project requires the NVCC compiler for CUDA and the g++ compiler for the PGM utility file. It also requires the `libjpeg` library for handling JPEG images. Please ensure these are installed and properly configured on your system before compiling and running the project.


## Authors

- [@JavRamCos](https://github.com/JavRamCos)
- [@AndresQuinto5](https://github.com/AndresQuinto5)
- [@CesarVin](https://github.com/CesarVin)

