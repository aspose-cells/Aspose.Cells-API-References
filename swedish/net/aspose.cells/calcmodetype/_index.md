---
title: "Enum CalcModeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CalcModeType enum. Representerar lägetypen för beräkning av formler"
type: docs
url: /sv/net/aspose.cells/calcmodetype/
---
## CalcModeType enumeration

Representerar lägesvarianten för beräkning av formler.

```csharp
public enum CalcModeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` |  |
| AutomaticExceptTable | `1` |  |
| Manual | `2` |  |

### Anmärkningar

Endast inställningar för MS Excel.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalcModeTypeDemo
    {
        public static void CalcModeTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för test
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

            // Åtkomst till formelinställningarna i arbetsboken
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Ställ in beräkningsläget till Manuell
            formulaSettings.CalculationMode = CalcModeType.Manual;

            // Ställ in andra formelinställningar
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

            // Spara arbetsboken
            workbook.Save("CalcModeTypeExample.xlsx");
            workbook.Save("CalcModeTypeExample.pdf");

        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


