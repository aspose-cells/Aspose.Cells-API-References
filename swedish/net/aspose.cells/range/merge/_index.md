---
title: "Range.Merge"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Kombinerar ett cellområde till en enda cell"
type: docs
url: /sv/net/aspose.cells/range/merge/
---
## Range.Merge method

Kombinerar ett cellområde till en enda cell.

```csharp
public void Merge()
```

### Anmärkningar

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i området.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMergeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett område och slå ihop celler (3 rader x 2 kolumner)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            range.Merge();

            // Ange värde i den sammanslagna cellen
            worksheet.Cells[0, 0].Value = "Merged Cells Demo";

            // Formatera de sammanslagna cellerna
            Style style = worksheet.Cells[0, 0].GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.IsBold = true;
            worksheet.Cells[0, 0].SetStyle(style);

            // Spara arbetsboken
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


