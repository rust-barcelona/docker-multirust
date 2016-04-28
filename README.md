A Docker image based on Ubuntu 16.04 that includes:

* [Multirust](https://github.com/brson/multirust)
* Aditional cross compile toolchains:
** arm-unknown-linux-gnueabi
** arm-unknown-linux-gnueabihf
** armv7-unknown-linux-gnueabihf
** aarch64-unknown-linux-gnu

This image allows to use Rust, Cargo, manage them with Multirust and cross compile to the included targets out of the box. 

## License

This repository is licensed the [MIT license](http://opensource.org/licenses/MIT).