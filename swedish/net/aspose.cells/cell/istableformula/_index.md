---
title: "Cell.IsTableFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑egenskap. Anger om den här cellen är en del av tabellformeln"
type: docs
url: /sv/net/aspose.cells/cell/istableformula/
---
## Cell.IsTableFormula property

Anger om den här cellen är en del av en tabellformel.

```csharp
public bool IsTableFormula { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellPropertyIsTableFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en tabell
            int index = worksheet.ListObjects.Add(0, 0, 5, 3, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Lägg till tabellformel i cell D2
            Cell cell = worksheet.Cells["D2"];
            cell.Formula = "=SUM(Table1[[#This Row],[Column1]:[Column3]])";
            
            // Kontrollera om cellen innehåller en tabellformel
            Console.WriteLine("Is table formula: " + cell.IsTableFormula);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


