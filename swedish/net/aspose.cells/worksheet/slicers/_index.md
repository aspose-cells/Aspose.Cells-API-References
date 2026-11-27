---
title: "Worksheet.Slicers"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Kalkylbladsattribut. Hämta Slicer-samlingen i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/slicers/
---
## Worksheet.Slicers property

Hämta Slicer-samlingen i arbetsbladet

```csharp
public SlicerCollection Slicers { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertySlicersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för tabellen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till en tabell
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Lägg till slicers i kalkylbladet
            worksheet.Slicers.Add(table, table.ListColumns[0], 1, 3);
            worksheet.Slicers.Add(table, 1, "D1");
            worksheet.Slicers.Add(table, table.ListColumns[0], "G1");

            // Spara arbetsboken
            workbook.Save("SlicersDemo.xlsx");
        }
    }
}
```

### Se även

* class [SlicerCollection](../../../aspose.cells.slicers/slicercollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


