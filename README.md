# SPOUT · task settings

Predefined per-task **CSV settings files** for **SPOUT** — part of the [spout-task](https://github.com/spout-task)
project. A settings file is the shareable, version-controllable definition of a task; the
MATLAB GUI in the [software](https://github.com/spout-task/software) repo loads it at run time, so parameters change
without recompiling firmware.

```
SPOUT1/  go_no_go/  stop_signal/  fixed_ratio/  progressive_ratio/  pavlovian/
SPOUT2/  uninstructed_ll_lr/  instructed_ll_lr/  two_armed_bandit/  delayed_response/  pavlovian/
```

## Format
A two-column CSV of `parameter,value` pairs (no header) — the same format written to
`*_Settings.csv` in a recorded session (see the [example_data](https://github.com/spout-task/example_data) repo). To
make one, configure a task in the GUI and save its settings, or copy and edit an existing file.

> **TODO:** drop the commonly-used settings CSV(s) into each task folder (5 for SPOUT1,
> 5 for SPOUT2). Folders currently hold a `.gitkeep` placeholder.

## License
**CC-BY-4.0** ([`LICENSE`](LICENSE)). See also [`CITATION.cff`](CITATION.cff).
