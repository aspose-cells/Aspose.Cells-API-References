---
title: "Cells.AddRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Lägger till en referens till ett områdeobjekt i cellerna"
type: docs
url: /sv/net/aspose.cells/cells/addrange/
---
## Cells.AddRange method

Lägger till en referens till ett områdeobjekt i celler.

```csharp
public void AddRange(Range rangeObject)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rangeObject | Range | Områdeobjektet kommer att finnas i cellerna |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodAddRangeWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in lite exempeldata i området
            cells["A1"].PutValue("A1");
            cells["A2"].PutValue("A2");
            cells["B1"].PutValue("B1");
            cells["B2"].PutValue("B2");

            // Skapa ett område och lägg till det med AddRange
            Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
            cells.AddRange(range);

            // Modifiera kalkylbladet för att demonstrera områdeutvidgning
            cells.InsertRow(1);
            cells.InsertColumn(1);

            Console.WriteLine($"Range now has {range.RowCount} rows and {range.ColumnCount} columns");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


