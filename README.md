# UART-Communication-Protocol
A simple 8-bit UART transmitter and receiver designed in Verilog and verified using Icarus Verilog and GTKWave.
# UART Communication Protocol in Verilog

## Overview

This project implements a basic **UART (Universal Asynchronous Receiver/Transmitter)** protocol using Verilog HDL. The system includes:

- **UART Transmitter (TX)**: Sends 8-bit serial data.
- **UART Receiver (RX)**: Receives 8-bit serial data.
- **UART Top Module**: Wraps TX and RX in a single module for easy integration.
- **Self-checking testbenches** using Icarus Verilog and GTKWave.

---

##  Tools Used

| Tool        | Purpose                      |
|-------------|------------------------------|
| Icarus Verilog (`iverilog`) | Simulation |
| GTKWave     | Waveform Viewer              |
| VS Code     | Source Code Editor           |

---

##  Project Structure
uart_project/
├── src/
│   ├── uart_tx.v             # UART Transmitter module
│   └── uart_rx.v             # UART Receiver module
│
├── tb/
│   ├── tb_uart_tx.v          # Testbench for UART Transmitter
│   ├── tb_uart_rx.v          # Testbench for UART Receiver
│   └── tb_uart_full.v        # Testbench for combined TX-RX system (if created)
│
├── sim/
│   ├── uart_tx_tb.vvp        # Compiled output for TX simulation
│   ├── uart_rx_tb.vvp        # Compiled output for RX simulation
│   ├── uart_full_tb.vvp      # Compiled output for full system simulation
│   ├── uart_tx.vcd           # Waveform for TX
│   ├── uart_rx.vcd           # Waveform for RX
│   └── uart_full.vcd         # Waveform for full system
│
├── images/
│   ├── uart_tx_wave.png      # Exported waveform image for TX
│   ├── uart_rx_wave.png      # Exported waveform image for RX
│   └── uart_combined_wave.png# Exported waveform for full system
