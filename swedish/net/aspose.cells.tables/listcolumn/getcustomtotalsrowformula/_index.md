---
title: "ListColumn.GetCustomTotalsRowFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn method. Hämtar formeln för totalsraden i den här listkolumnen"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/getcustomtotalsrowformula/
---
## ListColumn.GetCustomTotalsRowFormula method

Hämtar formeln för totalsraden för denna listkolumn.

```csharp
public string GetCustomTotalsRowFormula(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Returvärde

Formeln för den här listkolumnen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetCustomTotalsRowFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Ange anpassad totalsformel
            ListColumn listColumn = listObject.ListColumns[0];
            listColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Custom;
            listColumn.SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

            // Hämta och visa den anpassade totalsformeln
            string formula = listColumn.GetCustomTotalsRowFormula(false, true);
            Console.WriteLine("Custom Totals Formula: " + formula);

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


