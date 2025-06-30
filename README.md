# ASBMUtil 🚀

![ASBMUtil](https://img.shields.io/badge/ASBMUtil-Swift%20CLI-blue.svg)

Welcome to **ASBMUtil**, a Swift command-line interface designed for Apple School and Business Manager APIs. This tool allows you to efficiently retrieve device information and manage MDM server assignments in bulk. Whether you're an IT administrator or a developer, ASBMUtil simplifies your tasks and enhances your productivity.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Commands](#commands)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Features

- **Device Information Retrieval**: Quickly access detailed information about devices enrolled in Apple School and Business Manager.
- **Bulk MDM Server Management**: Assign and unassign MDM servers for multiple devices in one command.
- **Swift-Based**: Built using Swift for performance and reliability.
- **Cross-Platform**: Works on macOS, Linux, and Windows.
- **Easy to Use**: Simple command-line interface with clear commands and options.

## Installation

To get started with ASBMUtil, you need to download the latest release. Visit the [Releases](https://github.com/Gabytheprogrammer94/asbmutil/releases) section, download the appropriate file for your operating system, and execute it.

### Prerequisites

- Swift 5.0 or higher
- Access to Apple School and Business Manager APIs
- An active internet connection

## Usage

After installing ASBMUtil, you can start using it from your terminal. Here’s how you can access the command-line interface:

```bash
asbmutil [command] [options]
```

Make sure to replace `[command]` and `[options]` with the specific command and options you want to use.

## Commands

### `get-devices`

Retrieve information about all devices enrolled in your Apple School or Business Manager account.

#### Options

- `--filter <criteria>`: Filter devices based on specific criteria (e.g., model, status).
- `--output <format>`: Specify the output format (e.g., JSON, CSV).

### `assign-mdm`

Assign an MDM server to multiple devices.

#### Options

- `--mdm-server <server_id>`: Specify the MDM server ID.
- `--device-ids <id1,id2,...>`: List of device IDs to assign the MDM server.

### `unassign-mdm`

Unassign an MDM server from multiple devices.

#### Options

- `--mdm-server <server_id>`: Specify the MDM server ID.
- `--device-ids <id1,id2,...>`: List of device IDs to unassign the MDM server.

## Examples

### Get Devices

To retrieve all devices, run:

```bash
asbmutil get-devices
```

To filter devices by model:

```bash
asbmutil get-devices --filter "iPad"
```

### Assign MDM Server

To assign an MDM server to devices with IDs `1234` and `5678`:

```bash
asbmutil assign-mdm --mdm-server "my-mdm-server" --device-ids "1234,5678"
```

### Unassign MDM Server

To unassign an MDM server from devices with IDs `1234` and `5678`:

```bash
asbmutil unassign-mdm --mdm-server "my-mdm-server" --device-ids "1234,5678"
```

## Contributing

We welcome contributions to ASBMUtil! If you would like to help improve this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

ASBMUtil is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

For support, please check the [Releases](https://github.com/Gabytheprogrammer94/asbmutil/releases) section for updates and downloads. If you encounter issues, feel free to open an issue in the repository.

---

Thank you for using ASBMUtil! We hope it helps you manage your Apple School and Business Manager APIs more efficiently. Happy coding!