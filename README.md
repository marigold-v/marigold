# Marigold

Marigold is a free and open-source graphic creation suite.

## How to Build

The project is built using [CMake](https://cmake.org/), so make sure it is properly installed before building the project.

To get the source, simply clone the repository using [git](https://git-scm.com/):

```bash
git clone https://github.com/marigold-v/marigold.git
```

Then navigate to the source directory:

```bash
cd marigold
```

It's recommended to create a separate folder for the build files:

```bash
mkdir build && cd build
```

Generating the project files can be done with the following command. You can use a different configuration if you wish:

```bash
cmake -G "Visual Studio 16 2019" -A x64 ..
```

## Developer Forum

For discussions and support, join our [Discord](https://discord.gg/jDf2nphe4s)
