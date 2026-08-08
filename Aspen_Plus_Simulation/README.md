# Aspen Plus Simulation

## Model basis

The Aspen Plus simulation phase uses **Aspen Plus V14** with the **Electrolyte NRTL (ELECNRTL)** property method. The process basis supplied for the project is 10,000 kg/h industrial wastewater containing 2 wt% urea and 4 wt% KOH at 65 °C.

## Native model artifacts

`Base_Case/` contains the supplied Aspen project files:

- `Urea_Electrolyzer_Commercial_Finished_x2.bkp`
- `Urea_Electrolyzer_Commercial_Finished_x2.apw`
- `Urea_Electrolyzer_Commercial_Finished_x2.appdf`

These are retained in native format for reproducibility and inspection in a compatible Aspen Plus environment.

## Stream results

`Stream_Results/Latest Aspen Run Final Streams Table Results.xlsx` contains the supplied final stream-result export. The reported hydrogen product flow used in the project summary is **18.445 kg/h** (approximately 18.45 kg/h).

## Sensitivity studies

`Sensitivity_Analysis/` contains the supplied Excel exports for:

- Temperature sensitivity (`TEMP-SENS.xlsx`)
- Urea sensitivity (`UREA-SENS.xlsx`)
- KOH sensitivity (`KOH-SENS.xlsx`)

The files are preserved without altering the original numerical results.

## Flowsheet

`Flowsheet/Aspen_Process_Flowsheet.png` is the supplied Aspen process-flow-sheet image. It provides a visual overview of the electrolyzer and downstream gas/liquid separation, gas treatment/drying, and product/recovery streams.

## Viewing the files

The native Aspen files require **Aspen Plus V14 or a compatible Aspen Plus installation**. The `.xlsx` files can be inspected with Microsoft Excel, LibreOffice Calc, or another compatible spreadsheet application. The PNG flowsheet can be viewed directly in a browser.

## Reproducibility note

The repository preserves the supplied native model and exported results as source artifacts. Numerical results should be interpreted as simulation outputs unless an experimental validation artifact is explicitly identified elsewhere in the repository.
