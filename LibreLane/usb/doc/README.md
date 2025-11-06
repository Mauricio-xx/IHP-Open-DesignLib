# LibreLane USB Design

- **Design name:** `usb`
- **Configuration:** `design_data/librelane/config.json`
- **RTL sources:** `design_data/librelane/src/`
- **Validated flow:** LibreLane 3.0.0.dev39 + IHP SG13G2 commit 5fb50772cfe7c957a49eadb80c25aae3def38fe0

## Running the flow

1. Export `PDK_ROOT` to your SG13G2 checkout.
2. Activate the LibreLane Nix environment (`nix develop` inside the LibreLane repo).
3. Run:

```bash
librelane --run-tag ihp-sg13g2-usb \
  --pdk ihp-sg13g2 --scl sg13g2_stdcell \
  --pdk-root "$PDK_ROOT" --condensed \
  design_data/librelane/config.json
```

Results are written to `runs/ihp-sg13g2-usb`. Consult the IHP-Open-PDK documentation for
interpretation of the generated reports.
