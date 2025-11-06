# LibreLane Digital Examples

This directory collects RTL-to-GDS reference designs that have been validated with
LibreLane against the IHP SG13G2 PDK (commit `5fb50772cfe7c957a49eadb80c25aae3def38fe0`).
Each subdirectory follows the repository-wide convention (`design_data`, `doc`, `val`).

| Design       | Description                              | Notes |
|--------------|------------------------------------------|-------|
| `usb`        | USB full-speed device core                | Requires no external IP; runs with `sg13g2_stdcell` |
| `BM64`       | 64-bit Booth multiplier datapath          | Timing target relaxed to 30 ns |
| `picorv32a`  | PicoRV32 RISC-V microcontroller           | Stress test for larger block integration |

Refer to the documentation in `doc/README.md` inside each design for detailed build
instructions and links back to the official flow guide.
