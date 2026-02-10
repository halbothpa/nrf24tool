# Copilot Instructions for nrf24tool

## Project Overview

This is a **Flipper Zero** application written in **C** that interfaces with the NRF24L01+ transceiver module. It uses the **ufbt** (micro Flipper Build Tool) build system.

## Build System

- Build with: `ufbt build`
- Lint with: `ufbt lint`
- The app manifest is defined in `application.fam`
- Requires Flipper Zero firmware version **1.1.2** or higher

## Project Structure

- `nrf24tool.c` / `nrf24tool.h` — Main application entry point
- `gui.c` / `font.c` — GUI rendering and font data
- `helper.c` / `helper.h` — Utility functions
- `settings.c` / `settings.h` — Configuration management
- `libnrf24/` — NRF24L01+ hardware driver library
- `rx/` — Receive mode (RX)
- `tx/` — Transmit mode (TX)
- `sniff/` — Packet sniffer mode
- `badmouse/` — Mouse Jacker / BadUSB-like mode
- `documentation/` — Project documentation

## Coding Conventions

- C language (C11 compatible)
- Flipper Zero SDK APIs and Furi framework
- Use Flipper Zero's `furi_*` APIs for memory, logging, and threading
- Follow existing code style in the repository
