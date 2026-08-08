# Urea Wastewater Hydrogen Electrolyzer — Aspen Plus & Engineering Artifacts

Public engineering repository for the capstone project **Process Simulation, Prototyping, and Dynamic Control of Urea Wastewater Electrolysis for Green Hydrogen Production**.

## Project scope

This repository documents the process-simulation stage of a urea-containing industrial wastewater electrolysis system and will be expanded with CAD, calculations, process-design, safety, and experimental/prototyping artifacts in later phases.

### Aspen Plus model

- **Software:** Aspen Plus V14
- **Thermodynamics:** Electrolyte NRTL (`ELECNRTL`)
- **Design feed basis:** 10,000 kg/h industrial wastewater
- **Feed composition:** 2 wt% urea and 4 wt% KOH
- **Feed temperature:** 65 °C
- **Electrolyzer operating basis:** 1.5 V/cell
- **Stack basis:** 4 stacks × 40 cells/stack
- **DC power basis:** 800 kW
- **Reported final H₂ product flow:** 18.445 kg/h (approximately 18.45 kg/h)

The model represents urea wastewater electrolysis as an alternative anodic reaction pathway to conventional water oxidation, with downstream gas/liquid separation and hydrogen treatment represented in the process flowsheet.

## Repository structure

```text
.
├── Aspen_Plus_Simulation/
│   ├── Base_Case/
│   ├── Flowsheet/
│   ├── Sensitivity_Analysis/
│   ├── Stream_Results/
│   └── README.md
├── CAD_Models/                 # Phase 2
├── Calculations/               # Later phase
├── Process_Design/             # Later phase
├── Safety/                     # Later phase
├── Results/                    # Later phase
├── .gitignore
├── LICENSE
└── README.md
```

## Aspen Plus files

The `Aspen_Plus_Simulation` directory contains the native Aspen project artifacts, exported stream results, sensitivity studies, and the process-flow-sheet image supplied for this project. The native files are retained so that reviewers with compatible Aspen Plus installations can inspect the underlying model rather than relying only on screenshots.

See [`Aspen_Plus_Simulation/README.md`](Aspen_Plus_Simulation/README.md) for the detailed contents of this phase.

## Technical note

The quoted hydrogen production value is taken from the supplied final Aspen stream-results workbook. It is reported here as a **model result**, not as experimental validation. Experimental validation and further model refinement will be documented separately when those artifacts are added.

## Future phases

1. **Aspen Plus simulation** — current phase
2. **SolidWorks/CAD and neutral-format exports**
3. **Material and energy balances / engineering calculations**
4. **PFD, P&ID, controls, and process-design documentation**
5. **HAZOP and techno-economic analysis**
6. **Final portfolio documentation and reproducibility review**

## Citation and use

If you use material from this repository, please cite the project and identify the specific model, dataset, CAD artifact, or analysis used. Native Aspen and CAD files should be treated as engineering source artifacts and opened with the appropriate commercial software.

## License

Released under the MIT License. See [`LICENSE`](LICENSE).
