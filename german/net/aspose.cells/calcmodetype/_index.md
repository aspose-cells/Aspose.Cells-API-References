---
title: "Enum CalcModeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CalcModeType enum. Stellt den Modustyp für die Berechnung von Formeln dar."
type: docs
url: /de/net/aspose.cells/calcmodetype/
---
## CalcModeType enumeration

Stellt den Modustyp für die Berechnung von Formeln dar.

```csharp
public enum CalcModeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` |  |
| AutomaticExceptTable | `1` |  |
| Manual | `2` |  |

### Hinweise

Nur für MS Excel.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalcModeTypeDemo
    {
        public static void CalcModeTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für den Test hinzufügen
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

            // Greife auf die Formeleinstellungen der Arbeitsmappe zu
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Setze den Berechnungsmodus auf Manuell
            formulaSettings.CalculationMode = CalcModeType.Manual;

            // Setze weitere Formeleinstellungen
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

            // Speichere die Arbeitsmappe
            workbook.Save("CalcModeTypeExample.xlsx");
            workbook.Save("CalcModeTypeExample.pdf");

        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


