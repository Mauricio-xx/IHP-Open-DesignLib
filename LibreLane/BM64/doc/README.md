# LibreLane BM64 Design

- **Design name:** `BM64`
- **Configuration:** `design_data/librelane/config.json`
- **RTL sources:** `design_data/librelane/src/`
- **Validated flow:** LibreLane 3.0.0.dev39 + IHP SG13G2 commit 5fb50772cfe7c957a49eadb80c25aae3def38fe0

## Running the flow

```bash
librelane --run-tag ihp-sg13g2-bm64 \
  --pdk ihp-sg13g2 --scl sg13g2_stdcell \
  --pdk-root "$PDK_ROOT" --condensed \
  design_data/librelane/config.json
```

The configuration relaxes `CLOCK_PERIOD` to 30 ns and sets `FP_CORE_UTIL` to 18 to ensure
clean routing on SG13G2.
