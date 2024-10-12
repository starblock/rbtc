# rBTC - Bitcoin Client in Rust

**rBTC** is an implementation of the Bitcoin protocol written in Rust. This project aims to provide a lightweight, secure, and efficient Bitcoin client while taking advantage of Rust's memory safety and performance features.

## Features

- **Bitcoin Protocol**: Implements the Bitcoin protocol, allowing users to interact with the Bitcoin network.
- **Written in Rust**: Leverages the performance and safety features of Rust.
- **Requires Nightly Rust**: Due to certain experimental features and optimizations, rBTC requires the nightly version of Rust.

## Getting Started

### Prerequisites

- **Rust (Nightly)**: This project requires the nightly version of Rust. Install Rust and set up nightly toolchain:
  
  ```bash
  curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
  rustup install nightly
  rustup default nightly
  ```

- **Git**: Ensure Git is installed for cloning the repository.

### Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/rbtc.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd rbtc
   ```

3. **Build the project**:

   Compile the project using Rust's nightly toolchain:

   ```bash
   cargo +nightly build --release
   ```

4. **Run the Bitcoin client**:

   Once compiled, run the Bitcoin client:

   ```bash
   ./target/release/rbtc
   ```

### Configuration

rBTC uses a simple configuration file `rbtc.conf` for setting up network parameters, peers, and other options. Modify this file as necessary for your network setup.

### Usage

After starting the client, it will attempt to connect to the Bitcoin network and synchronize the blockchain.

Common commands:
```bash
./rbtc --help        # Display help and available commands
./rbtc --sync        # Start syncing with the Bitcoin network
./rbtc --balance     # Show your wallet balance
```

### Development

If you're contributing to rBTC or developing new features, you can use the following command to run the project in debug mode:

```bash
cargo +nightly run
```

### Testing

To run the unit tests:

```bash
cargo +nightly test
```

### Contributing

We welcome contributions! If you'd like to contribute, follow these steps:

1. **Fork the repository**.
2. **Create a new branch** (`git checkout -b feature-branch`).
3. **Make your changes** and commit them (`git commit -m 'Add new feature'`).
4. **Push to your branch** (`git push origin feature-branch`).
5. **Open a pull request** and describe your changes.

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
