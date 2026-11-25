---
title: "Classe FormulaSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FormulaSettings. Impostazioni delle formule e del calcolo"
type: docs
url: /it/net/aspose.cells/formulasettings/
---
## FormulaSettings class

Impostazioni delle formule e del calcolo.

```csharp
public class FormulaSettings
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CalculateOnOpen](../../aspose.cells/formulasettings/calculateonopen/) { get; set; } | Indica se l'applicazione deve eseguire un calcolo completo quando la cartella di lavoro viene aperta. |
| [CalculateOnSave](../../aspose.cells/formulasettings/calculateonsave/) { get; set; } | Indica se ricalcolare la cartella di lavoro prima di salvare il documento, quando è in modalità di calcolo manuale. |
| [CalculationId](../../aspose.cells/formulasettings/calculationid/) { get; set; } | Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro. |
| [CalculationMode](../../aspose.cells/formulasettings/calculationmode/) { get; set; } | Ottiene o imposta la modalità di calcolo della cartella di lavoro in MS Excel. |
| [EnableCalculationChain](../../aspose.cells/formulasettings/enablecalculationchain/) { get; set; } | Indica se abilitare la catena di calcolo per le formule. Il valore predefinito è false. |
| [EnableIterativeCalculation](../../aspose.cells/formulasettings/enableiterativecalculation/) { get; set; } | Indica se abilitare il calcolo iterativo per risolvere riferimenti circolari. |
| [ForceFullCalculation](../../aspose.cells/formulasettings/forcefullcalculation/) { get; set; } | Indica se calcola tutte le formule ogni volta che viene avviato un calcolo. |
| [MaxChange](../../aspose.cells/formulasettings/maxchange/) { get; set; } | La variazione massima per risolvere un riferimento circolare. |
| [MaxIteration](../../aspose.cells/formulasettings/maxiteration/) { get; set; } | Il numero massimo di iterazioni per risolvere un riferimento circolare. |
| [PrecisionAsDisplayed](../../aspose.cells/formulasettings/precisionasdisplayed/) { get; set; } | Indica se la precisione del risultato calcolato deve essere impostata così come viene visualizzata durante il calcolo delle formule. |
| [PreservePaddingSpaces](../../aspose.cells/formulasettings/preservepaddingspaces/) { get; set; } | Indica se conservare gli spazi e le interruzioni di riga inseriti tra i token delle formule durante il recupero e l'impostazione delle formule. Il valore predefinito è false. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaSettingsDemo
    {
        public static void FormulaSettingsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle impostazioni delle formule della cartella di lavoro
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Impostazione delle proprietà
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationMode = CalcModeType.Automatic;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Salva la cartella di lavoro
            workbook.Save("FormulaSettingsExample.xlsx");
            workbook.Save("FormulaSettingsExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


