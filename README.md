A Docker image based on Ubuntu 16.04 that includes:

* [Multirust](https://github.com/brson/multirust)
* Aditional cross compile toolchains:
  * arm-unknown-linux-gnueabi
  * arm-unknown-linux-gnueabihf
  * armv7-unknown-linux-gnueabihf
  * aarch64-unknown-linux-gnu

This image allows to use Rust, Cargo, manage them with Multirust and cross compile to the included targets out of the box. 

## Usage

Once the image has been built, an interactive session will allow to use the usual commands: cargo, rustc, multirust, rustdoc, etc.

The interactive session needs to bind the working directory in the host machine and the workspace directory in the image:

Generically:
```bash
docker run -it --rm -v [path_project_directory]:/workspace rustbarcelona/docker-multirust
```

To bind the current folder:
```bash
docker run -it --rm -v $(pwd):/workspace rustbarcelona/docker-multirust
```

After this step is completed, a bash session is established on the guest system, in the /workspace folder.


## License

This repository is licensed the [MIT license](http://opensource.org/licenses/MIT).