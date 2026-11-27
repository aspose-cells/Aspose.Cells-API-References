---
title: "Range.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑egenskap. Hämtar Cell‑objektet i detta område"
type: docs
url: /sv/net/aspose.cells/range/item/
---
## Range indexer

Hämtar ett [`Cell`](../../cell/)‑objekt i detta område.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| rowOffset | Radoffset i detta intervall, nollbaserat. |
| columnOffset | Kolumnoffset i detta intervall, nollbaserat. |

### Returvärde

[`Cell`](../../cell/) object.

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangePropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata
            DataTable dt = new DataTable();
            dt.Columns.Add("Id", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Rows.Add(1001, "Item 1");
            dt.Rows.Add(1002, "Item 2");

            // Skapa ett område och demonstrera Item‑egenskapen
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B3");
            
            // Ställ in rubriker med Item‑egenskapen
            range[0, 0].PutValue("Id");
            range[0, 1].PutValue("Name");

            // Fyll data med Item-egenskapen
            for (int i = 0; i < dt.Rows.Count; i++)
            {
                range[i + 1, 0].PutValue(dt.Rows[i]["Id"]);
                range[i + 1, 1].PutValue(dt.Rows[i]["Name"]);
            }

            // Formatera rubrikrad med Item-egenskapen
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.FromArgb(0, 176, 80);
            range[0, 0].SetStyle(style);
            range[0, 1].SetStyle(style);

            // Spara arbetsboken
            workbook.Save("RangePropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


