# Rust OpenGL Window Example

![Rust Logo](https://www.rust-lang.org/static/images/rust-logo-blk.svg)

This is a simple Rust project named **RustGLWindow** that demonstrates how to create a basic OpenGL window using Rust. The project is designed to be used with Visual Studio Code's DevContainer, making it easy to set up a development environment for OpenGL programming in Rust on Linux.

## Prerequisites

Before you begin, make sure you have the following tools installed on your Linux system:

- [Visual Studio Code](https://code.visualstudio.com/)
- [Docker](https://www.docker.com/)

## Getting Started

Follow these steps to set up the development environment and run the Rust OpenGL window example:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/Ruj89/RustGLWindow.git
   ```

2. Customize and move the `devcontainer.json.template` file to `.devcontainer/devcontainer.json`.

3. Open Visual Studio Code (VSCode) and navigate to the project folder:

   ```bash
   code RustGLWindow
   ```

4. When you open the project in VSCode, it will detect the DevContainer configuration and ask if you want to reopen the project in a container. Select "Reopen in Container" to set up the development environment.

5. Wait for VSCode to build and configure the DevContainer. This might take a few moments.

6. Once the DevContainer is set up, you can build and run the Rust OpenGL window example using the integrated terminal:

   ```bash
   cargo run
   ```

7. The OpenGL window should open, displaying a simple colored triangle.

## Project Structure

The project has the following structure:

- `lib/` - Contains the project libraries.
  - `lib/gl` - Contains the OpenGL library.
    - `src/` - Contains the Rust source code for the OpenGL library.
      - `lib.rs` - The library bindings.
    - `build.rs` - The bindings build script.
    - `Cargo.toml` - The Rust package manager configuration file for the library.
    - `Cargo.lock` - The Rust package manager lock file for the library.
- `shaders/` - Contains the example shaders.
  - `triangle.frag` - The fragment shader.
  - `triangle.vert` - The vertex shader.
- `src/` - Contains the Rust source code for the OpenGL window example.
  - `main.rs` - The main entry point for the application.
  - `render_gl.rs` - The OpenGL program.
  - `resources.rs` - Resource files loader.
- `devcontainer.json.template` - Configures the development environment for VSCode.
- `Cargo.toml` - The Rust package manager configuration file.
- `Cargo.lock` - The Rust package manager lock file.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to [nercury](https://nercury.github.io/) for his [OpenGL tutorial](https://nercury.github.io/rust/opengl/tutorial/2018/02/12/opengl-in-rust-from-scratch-06-gl-generator.html)
- This project was inspired by the great Rust and OpenGL community.
- Thanks to the Visual Studio Code team for their excellent DevContainer support.

## Contributing

If you'd like to contribute to this project, feel free to fork it and submit a pull request. We welcome contributions and feedback from the community.

Happy coding!