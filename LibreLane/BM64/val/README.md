# Validation Notes

Tool versions:

- LibreLane 3.0.0.dev39
- Yosys 0.54
- OpenROAD build 2025-09-01
- Magic 8.3.528
- Verilator 5.038
- KLayout 0.30.2

The BM64 run achieved clean STA with `CLOCK_PERIOD = 30` ns. DRC and LVS were clean using
LibreLane's Magic + Netgen steps and the SG13G2 KLayout deck.
