---
title: "CellArea.StartColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellArea-fält. Hämtar eller anger startkolumnen för detta område"
type: docs
url: /sv/net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Hämtar eller anger startkolumnen för detta område.

```csharp
public int StartColumn;
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange viss initial data
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);

            // Skapa ett CellArea och ange dess StartColumn
            CellArea area = new CellArea();
            area.StartRow = 1;
            area.EndRow = 3;
            area.StartColumn = 0; // Using StartColumn field
            area.EndColumn = 0;

            // Infoga en ny kolumn genom att flytta befintliga celler nedåt
            cells.InsertRange(area, ShiftType.Down);

            // Verifiera resultatet
            Console.WriteLine("A1 value: " + cells["A1"].StringValue); // Should be empty
            Console.WriteLine("A2 value: " + cells["A2"].StringValue); // Should be "Header"
            Console.WriteLine("A3 value: " + cells["A3"].IntValue); // Should be 10
        }
    }
}
```

### Se även

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


