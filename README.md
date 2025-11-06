# IHP-Open-DesignLib
Open source designs developed with IHP 130nm BiCMOS Open Source PDK

ReadTheDocs documentation for IHP-Open-DesignLib is [here](https://ihp-open-ip.readthedocs.io/en/latest/)

Proposed directory structure:
```text
📁<design_name>
 ┣ 📁design_data
 ┃ ┗ ...
 ┣ 📁doc
 ┃ ┣ 📜specification
 ┃ ┣ ...
 ┗ 📁val <- validation/verification
 ```

## Directory overview

- `AnalogLDO_exampleDesign`, `LNA_24GHz`, etc.: analogue reference designs.
- `LibreLane/`: digital RTL-to-GDS examples validated with LibreLane + SG13G2. See
  `LibreLane/README.md` for the list of currently supported designs (`usb`, `BM64`,
  `picorv32a`).
