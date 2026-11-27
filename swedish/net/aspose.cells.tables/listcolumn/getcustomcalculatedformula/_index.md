---
title: "ListColumn.GetCustomCalculatedFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn method. Hämtar formeln för den här listkolumnen"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/getcustomcalculatedformula/
---
## ListColumn.GetCustomCalculatedFormula method

Hämtar formeln för denna listkolumn.

```csharp
public string GetCustomCalculatedFormula(bool isR1C1, bool isLocal)
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
    public class ListColumnMethodGetCustomCalculatedFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Skapa exempeldata
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B1"].PutValue("Score");
            sheet.Cells["B2"].PutValue(85);
            sheet.Cells["B3"].PutValue(92);
            
            // Skapa ett listobjekt
            int index = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = sheet.ListObjects[index];
            
            // Lägg till en beräknad kolumn
            ListColumn calcColumn = listObject.ListColumns[1];
            calcColumn.Formula = "=WEEKNUM([@Score])";
            
            // Hämta den anpassade beräknade formeln
            string formula = listObject.ListColumns[1].GetCustomCalculatedFormula(false, false);
            
            // Skriv ut resultatet
            Console.WriteLine("Calculated Formula: " + formula);
        }
    }
}
```

### Se även

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


