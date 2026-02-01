# 🟦 KINETIC DRIVE

**KINETIC DRIVE** is a high-performance terminal user interface (TUI) that reimagines the "hypnotic satisfaction" of 90s disk defragmentation for modern storage architecture.

While modern SSDs lack moving parts, they are a hive of activity—TRIM commands, wear leveling, and garbage collection. This tool abstracts complex NVMe/SSD telemetry into a "Ghost-Motion" grid, providing a visual bridge between the mechanical past and the high-velocity silicon present.

---

## 🛠 Features

* **Kinetic Visualization:** A real-time, low-latency grid mapping Logical Block Addresses (LBA) to your terminal.
* **The "Fake" Motion Engine:** An optional simulation layer that mimics physical head movement and data relocation for purely aesthetic satisfaction.
* **Telemetry Integration:** Interfaces with macOS `diskutil` and Windows Storage APIs to visualize actual I/O throughput.
* **Low-Overhead:** Written in **Rust** with a zero-allocation rendering loop to ensure the monitor doesn't interfere with the drive's actual performance.
* **Aesthetic Presets:** Includes `Classic-DOS` (Blue/White), `Matrix` (Neon Green), and `Cyberpunk` (High-contrast Magenta).

## 🚀 Tech Stack

* **Core:** [Rust](https://www.rust-lang.org/)
* **UI Framework:** [Ratatui](https://ratatui.rs/) / `crossterm`
* **Telemetry:** Custom `ioctl` wrappers for macOS and `Win32` storage handles for Windows.

## 📦 Installation

### Prerequisites

* Rust toolchain (Cargo)
* Administrator/Root privileges (Required for low-level disk access)

### Build

```bash
# Clone the repository
git clone https://github.com/makalin/kinetic-drive
cd kinetic-drive

# Build for release
cargo build --release

# Run KINETIC DRIVE
sudo ./target/release/kinetic-drive

```

## 🎮 Usage

| Key | Action |
| --- | --- |
| `Space` | Toggle "Ghost-Motion" (Simulation Mode) |
| `T` | Cycle Color Themes |
| `S` | Toggle Statistics Overlay |
| `Q` / `Esc` | Exit Application |

## ⚠️ Disclaimer

**KINETIC DRIVE is a visualization and monitoring tool.** Modern SSDs should **never** be defragmented in the traditional sense. This software does not physically move data in a way that harms flash memory; it merely visualizes existing system operations (TRIM/GC) or simulates movement for aesthetic purposes.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

---

**License:** MIT

**Author:** Mehmet T. AKALIN ([@makalin](https://github.com/makalin))

**Company:** [Digital Vision](https://dv.com.tr)
