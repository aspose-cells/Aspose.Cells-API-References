---
title: "Row.IsHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Anger om raden är dold"
type: docs
url: /sv/net/aspose.cells/row/ishidden/
---
## Row.IsHidden property

Anger om raden är dold.

```csharp
public bool IsHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                cells[$"A{i + 1}"].PutValue($"Row {i + 1}");
            }

            // Dölj några rader
            cells.HideRow(2);  // Row 3 (0-based index 2)
            cells.HideRow(5);  // Row 6 (0-based index 5)
            cells.HideRow(8);  // Row 9 (0-based index 8)

            // Kontrollera och visa IsHidden-status för varje rad
            for (int i = 0; i < 10; i++)
            {
                bool isHidden = cells.Rows[i].IsHidden;
                Console.WriteLine($"Row {i + 1} is hidden: {isHidden}");
            }

            // Spara arbetsboken
            workbook.Save("RowHiddenDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


