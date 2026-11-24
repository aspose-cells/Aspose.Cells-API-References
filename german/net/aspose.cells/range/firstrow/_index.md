---
title: "Range.FirstRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt den Index der ersten Zeile des Bereichs zurück"
type: docs
url: /de/net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

Liefert den Index der ersten Zeile des Bereichs.

```csharp
public int FirstRow { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und greifen Sie auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten befüllen
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Erstelle einen Bereich
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Greifen Sie auf die FirstRow-Eigenschaft zu und zeigen Sie sie an
            Console.WriteLine("First row index of range: " + range.FirstRow);

            // Greifen Sie auf die erste Zelle in der ersten Zeile des Bereichs zu
            Cell firstCell = worksheet.Cells[range.FirstRow, range.FirstColumn];
            Console.WriteLine("First cell value: " + firstCell.StringValue);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


