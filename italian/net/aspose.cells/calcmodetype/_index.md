---
title: "Enum CalcModeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.CalcModeType enum. Rappresenta il tipo di modalità di calcolo delle formule"
type: docs
url: /it/net/aspose.cells/calcmodetype/
---
## CalcModeType enumeration

Rappresenta il tipo di modalità di calcolo delle formule.

```csharp
public enum CalcModeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` |  |
| AutomaticExceptTable | `1` |  |
| Manual | `2` |  |

### Osservazioni

Solo impostazioni per MS Excel.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalcModeTypeDemo
    {
        public static void CalcModeTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il test
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            worksheet.Cells["A4"].Formula = "=A1+B1+C1";
            worksheet.Cells["B4"].Formula = "=SUM(B1:B3)";

            // Accedi alle impostazioni della formula della cartella di lavoro
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Imposta la modalità di calcolo su Manuale
            formulaSettings.CalculationMode = CalcModeType.Manual;

            // Imposta altre impostazioni della formula
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Salva la cartella di lavoro
            workbook.Save("CalcModeTypeExample.xlsx");
            workbook.Save("CalcModeTypeExample.pdf");

        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


