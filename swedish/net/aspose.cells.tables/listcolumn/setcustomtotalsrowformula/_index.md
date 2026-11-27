---
title: "ListColumn.SetCustomTotalsRowFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn method. Hämtar formeln för totalsraden i den här listkolumnen"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/setcustomtotalsrowformula/
---
## ListColumn.SetCustomTotalsRowFormula method

Hämtar formeln för totalsraden för denna listkolumn.

```csharp
public void SetCustomTotalsRowFormula(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | formeln för den här listkolumnen. |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetCustomTotalsRowFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Aktivera totalsrad och ange anpassad formel
            listObject.ShowTotals = true;
            listObject.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
            listObject.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


