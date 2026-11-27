---
title: "Worksheet.ConvertFormulaReferenceStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Konverterar formelns referensstil"
type: docs
url: /sv/net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

Konverterar formelreferensstilen.

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formeln som ska konverteras. |
| toR1C1 | Boolean | Vilken referensstil formeln ska konverteras till. Om den ursprungliga formeln är i A1-referensstil, bör detta värde vara true så att formeln konverteras från A1 till R1C1-referensstil; om den ursprungliga formeln är i R1C1-referensstil, bör detta värde vara false så att formeln konverteras från R1C1 till A1-referensstil; |
| baseCellRow | Int32 | Radindex för bascellen. |
| baseCellColumn | Int32 | Kolumnindex för bascellen. |

### Returvärde

Den konverterade formeln.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Exempel 1: Konvertera R1C1-stil till A1-stil
            string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
            string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
            Console.WriteLine("Converted formula: " + formulaA1);

            // Exempel 2: Konvertera med blandade referenser
            string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
            string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
            Console.WriteLine("Converted mixed formula: " + convertedMixed);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


