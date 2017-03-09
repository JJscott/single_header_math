# cgra_math.hpp

[cgra_math.hpp](/cgra_math.hpp) is a single header math library containing data structures and functions for applications in computer graphics, computational geometry and physical simulation. It serves as a light-weight alternative to [GLM](http://glm.g-truc.net/) or [Eigen](http://eigen.tuxfamily.org/) and is inspired by the functionality and style of [GLSL](https://www.opengl.org/registry/); designed to be fast, flexible and easy-to-use.


# FAQ

#### Why did you make another math library?

There are a large number of existing libraries for linear algebra in C++ but the majority of them are slow to compile and  complicated to integrate. `cgra_math.hpp` is a single header file that provides a variety of data types and functions that most suitable for applications in Computer Graphics. It can be integrated straight into your source tree without any hassle.

#### Why C++11?

TODO

#### Why are Matrices Column-major?

TODO
Originally this library was developed for use in OpenGL which requires the data to be packed in column major order.
Array subscript operator allows you to access the matrix by column then row (x then y) which is easier for beginners to understand. A single array subscript operator also allows us to return a reinterpret cast of the data as a vector with length equal to the number of rows making it easier to modify.


# Documentation

* [Scalars](#scalars)
* [Data Structures](#data-structures)
* [Operator Overloads](#operator-overloads)
* [Angle and Trigonometry Functions](#angle-and-trigonometry-functions)
* [Exponential Functions](#exponential-functions)
* [Common Functions](#common-functions)
* [Packing Functions](#packing-functions)
* [Geometric Functions](#geometric-functions)
* [Relational Functions](#relational-functions)
* [Integer Functions](#integer-functions)
* [Matrix Functions](#matrix-functions)
* [Transform Functions](#transform-functions)
* [Quaternion Functions](#quaternion-functions)
* [Higher Order Functions](#higher-order-functions)


## Scalars

## Data Structures

### `basic_vec<T, N>`
TODO constructors
TODO operators
TODO explicit template override

### `basic_mat<T, N>`
Data is stored in column major order
TODO constructors
TODO operators

### `basic_quat<T, N>`
TODO constructors
TODO operators

### Aliases

A number of convenient aliases, which can be brought into scope with a `using` declaration. The typedefs for `float` based vectors and matrices are shown below GLSL naming scheme (default):

|    Type    | `basic_vec<T, N>` | `basic_mat<T, N, N>` | `basic_mat<T, M, N>` | `basic_quat<T>` |
|:----------:|:-----------------:|:--------------------:|:--------------------:|:---------------:|
|   *float*  |       `vecN`      |        `matN`        |       `matMxN`       |      `quat`     |
|  *double*  |      `dvecN`      |        `dmatN`       |       `dmatMxN`      |     `dquat`     |
|    *int*   |      `ivecN`      |        `imatN`       |       `imatMxN`      |                 |
| *unsigned* |      `uvecN`      |                      |                      |                 |
|   *bool*   |      `bvecN`      |                      |                      |                 |

Initial3D naming scheme

|    Type    | `basic_vec<T, N>` | `basic_mat<T, N, N>` | `basic_mat<T, M, N>` | `basic_quat<T>` |
|:----------:|:-----------------:|:--------------------:|:--------------------:|:---------------:|
|   *float*  |      `vecNf`      |        `matNf`       |       `matMxNf`      |     `quatf`     |
|  *double*  |      `vecNd`      |        `matNd`       |       `matMxNd`      |     `quatd`     |
|    *int*   |      `vecNi`      |        `matNi`       |       `matMxNi`      |                 |
| *unsigned* |      `vecNu`      |                      |                      |                 |
|   *bool*   |      `vecNb`      |                      |                      |                 |

HLSL naming scheme (TODO)

|    Type    | `basic_vec<T, N>` | `basic_mat<T, M, N>` |
|:----------:|:-----------------:|:--------------------:|
|   *float*  |      `floatN`     |      `floatMxN`      |
|  *double*  |     `doubleN`     |      `doubleMxN`     |
|    *int*   |       `intN`      |       `intMxN`       |
| *unsigned* |      `uintN`      |                      |
|   *bool*   |      `boolN`      |                      |


## Operator Overloads

TODO

## Angle and Trigonometry Functions

TODO

## Exponential Functions

TODO

## Common Functions

TODO

## Packing Functions

TODO

## Geometric Functions

TODO

## Relational Functions

TODO

## Integer Functions

TODO

## Matrix Functions

TODO

## Transform Functions

TODO

## Quaternion Functions

TODO

## Higher Order Functions

TODO

# Running the Testing Suite

TODO

# Acknowledgments

TODO