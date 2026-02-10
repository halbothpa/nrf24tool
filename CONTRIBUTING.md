# Contributing to nrf24tool

Thank you for your interest in contributing to nrf24tool! This document provides guidelines to help you get started.

## Getting Started

1. **Fork** this repository
2. **Clone** your fork:
   ```bash
   git clone https://github.com/<your-username>/nrf24tool.git
   cd nrf24tool
   ```
3. Create a new **branch** for your feature or fix:
   ```bash
   git checkout -b feature/my-feature
   ```

## Build & Lint

This project uses [ufbt](https://github.com/flipperdevices/flipperzero-ufbt) (micro Flipper Build Tool).

```bash
# Build the application
ufbt build

# Lint source code
ufbt lint
```

> **Note:** Requires Flipper Zero firmware version **1.1.2** or higher.

## Project Structure

| Path | Description |
|------|-------------|
| `nrf24tool.c` / `nrf24tool.h` | Main application entry point |
| `gui.c` / `font.c` | GUI rendering and font data |
| `helper.c` / `helper.h` | Utility functions |
| `settings.c` / `settings.h` | Configuration management |
| `libnrf24/` | NRF24L01+ hardware driver library |
| `rx/` | Receive mode |
| `tx/` | Transmit mode |
| `sniff/` | Packet sniffer mode |
| `badmouse/` | Mouse Jacker / BadUSB-like mode |
| `documentation/` | Project documentation |

## Coding Conventions

- C language (C11 compatible)
- Use Flipper Zero SDK APIs and Furi framework (`furi_*` APIs)
- Follow the existing code style in the repository
- Keep changes minimal and focused

## Submitting Changes

1. Commit your changes with clear, descriptive messages
2. Push to your fork
3. Open a **Pull Request** against the `main` branch
4. Describe what your changes do and why

## Reporting Issues

- Use the [Bug Report](../../issues/new?template=bug_report.md) template for bugs
- Use the [Feature Request](../../issues/new?template=feature_request.md) template for enhancements
- Check [KNOWN_ISSUES.md](KNOWN_ISSUES.md) before reporting

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE).
