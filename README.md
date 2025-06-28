# button-no-std
# ESP32 Button Interrupt Example (Rust `no_std`)

This is a simple embedded Rust project for the ESP32-C3 that demonstrates how to configure:
- A GPIO output pin (LED)
- A GPIO input pin (button)
- An interrupt handler for button events
- `no_std` environment with HAL and critical sections

---

## 🔧 Hardware Requirements

- ESP32-C3 development board (e.g. ESP32-C3-DevKitM-1)
- Push button connected to GPIO9
- LED connected to GPIO7
- Optionally, a pull-up resistor on the button

---

## 🛠️ Features

- Rust embedded with `#![no_std]`
- GPIO interrupt handling with a safe `Mutex`
- Uses `esp-hal`, `esp-backtrace`, and `esp-println` for HAL and debugging
- Prints to serial on button press (interrupt triggered)

---

## 🚀 How to Build and Flash

### 1. Prerequisites

- Rust nightly toolchain
- `espup` and `espflash` installed
- Set up the ESP32 Rust env
