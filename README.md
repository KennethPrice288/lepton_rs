# lepton_rs

![Build Status](https://github.com/KennethPrice288/lepton_rs/actions/workflows/ci.yml/badge.svg)
![Crates.io](https://img.shields.io/crates/v/lepton_rs)
![Docs.rs](https://docs.rs/lepton_rs/badge.svg)

`lepton_rs` is a Rust library providing a device driver for the Lepton thermal camera. This crate allows you to interface with the Lepton camera, capture images, and process thermal data.

## Features

-  Interface with Lepton thermal cameras
-  Capture thermal images
-  Process and analyze thermal data
-  Easy-to-use API

## Installation

Add `lepton_rs` to your `Cargo.toml`:

```toml
[dependencies]
lepton_rs = "0.1.0"
Then, run cargo build to download and compile the crate.
Usage
Here's a basic example of how to use lepton_rs:

use lepton_rs::LeptonCamera;

fn main() {
    // Initialize the Lepton camera
    let mut camera = LeptonCamera::new().expect("Failed to initialize the camera");

    // Capture an image
    let image = camera.capture().expect("Failed to capture image");

    // Process the image
    // (Add your image processing code here)

    println!("Image captured successfully!");
}
Documentation
Full documentation is available on docs.rs.
Examples
You can find more examples in the examples directory.
Contributing
Contributions are welcome! Please see the CONTRIBUTING.md for more details.
License
This project is licensed under the MIT License. See the LICENSE file for details.
Contact
For questions, suggestions, or issues, please open an issue on the GitHub repository.
￼Note: This crate is in active development. Features and APIs are subject to change.
