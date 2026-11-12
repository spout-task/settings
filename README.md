# SPOUT task settings

Predefined **CSV settings files** for **SPOUT**, part of the [spout-task](https://github.com/spout-task) project.
A settings file defines a task completely. The MATLAB GUI in the [software](https://github.com/spout-task/software)
repository loads it with **Load settings** and sends it to the Teensy, so you can switch tasks and
change parameters without recompiling the firmware.

## Contents

```
SPOUT1/
  Pavlovian/
    Pavlovian_stage1.csv
SPOUT2/
  uninstructed_LL-LR/
    uninstructed_LL-LR_stage4.csv
```

| File | System | Task | What it is |
|---|---|---|---|
| [`SPOUT1/Pavlovian/Pavlovian_stage1.csv`](SPOUT1/Pavlovian/Pavlovian_stage1.csv) | SPOUT1 | Pavlovian conditioning | Training stage 1 |
| [`SPOUT2/uninstructed_LL-LR/uninstructed_LL-LR_stage4.csv`](SPOUT2/uninstructed_LL-LR/uninstructed_LL-LR_stage4.csv) | SPOUT2 | Uninstructed lick left, lick right | Training stage 4 |

A library with settings files for every task and training stage is in preparation and will be added
here, one folder per task.

## Format

A two column CSV of `parameter,value` pairs without a header. It uses the same parameter names as the
`*_Settings.csv` file written for every recorded session (see the
[example_data](https://github.com/spout-task/example_data) repository), without the session information
rows. To make your own, set up a task in the GUI and save its settings, or copy and edit an existing file.

## License
**CC-BY-4.0** ([`LICENSE`](LICENSE)). See also [`CITATION.cff`](CITATION.cff).
