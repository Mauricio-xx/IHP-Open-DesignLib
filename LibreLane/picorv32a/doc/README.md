# LibreLane picorv32a Design

- **Design name:** `picorv32a`
- **Configuration:** `design_data/librelane/config.json`
- **RTL sources:** `design_data/librelane/src/`
- **Validated flow:** LibreLane 3.0.0.dev39 + IHP SG13G2 commit 5fb50772cfe7c957a49eadb80c25aae3def38fe0

## Running the flow

```bash
librelane --run-tag ihp-sg13g2-picorv32a \
  --pdk ihp-sg13g2 --scl sg13g2_stdcell \
  --pdk-root "$PDK_ROOT" --condensed \
  design_data/librelane/config.json
```

This design stresses placement, routing, and timing optimisation with ~46k instances. The
configuration relies on SG13G2 overrides inside the JSON file.
