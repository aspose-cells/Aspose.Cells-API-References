---
title: "DataSorterKey.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorterKey‑egenskap. Hämtar den sorterade färgen"
type: docs
url: /sv/net/aspose.cells/datasorterkey/color/
---
## DataSorterKey.Color property

Hämtar den sorterade färgen.

```csharp
public Color Color { get; }
```

### Anmärkningar

Gäller endast när [`Type`](../type/) är CellColor eller FontColor.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyColorDemo
    {
        public static void Run()
        {
            // Skapa ett arbetsbok-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Skapa datasortering och lägg till nyckel
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Sortera data
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Skriv ut färgegenskapen från nycklarna
            foreach (DataSorterKey k in sorter.Keys)
            {
                Console.WriteLine($"Color: {k.Color}");
            }
        }
    }
}
```

### Se även

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


