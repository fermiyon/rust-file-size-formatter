![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
## Date Created

9 June 2024

# File Size Converter

This Rust program provides a simple way to convert file sizes between different units of measurement. It supports bytes, kilobytes, megabytes, and gigabytes.

## Features

- Parse file size input from the command line.
- Convert file sizes to various units.
- Display converted sizes in a human-readable format.

## Usage

To use this program, you need to pass the file size with its unit as an argument when running the program. The format should be `<size> <unit>`, where `<unit>` can be `bytes`, `kb`, `mb`, or `gb`.

```bash
cargo run -- 300 kb
```

Running the command above will produce the following output:

```bash
Bytes: 300000 bytes
Kilobytes: 300.00 KB
Megabytes: 0.30 MB
Gigabytes: 0.00 GB
Sizes: Sizes { bytes: "300000 bytes", kilobytes: "300.00 KB", megabytes: "0.30 MB", gigabytes: "0.00 GB" }
```

## Implementation Details

Implementation Details
The program defines an enum called FileSize that represents the file size in different units. It also includes a struct called Sizes that formats the file size into strings for each unit.

The FileSize::from_input function parses the input string and returns the corresponding FileSize. The Sizes::from_file_size function takes a FileSize and returns a Sizes instance with formatted strings for each unit.

## Author
Selman Karaosmanoglu

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.

## Credits

Coursera Rust Fundementals Program