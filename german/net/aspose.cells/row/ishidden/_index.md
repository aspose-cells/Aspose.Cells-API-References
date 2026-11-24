---
title: "Row.IsHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Eigenschaft. Gibt an, ob die Zeile ausgeblendet ist"
type: docs
url: /de/net/aspose.cells/row/ishidden/
---
## Row.IsHidden property

Gibt an, ob die Zeile ausgeblendet ist.

```csharp
public bool IsHidden { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                cells[$"A{i + 1}"].PutValue($"Row {i + 1}");
            }

            // Einige Zeilen ausblenden
            cells.HideRow(2);  // Row 3 (0-based index 2)
            cells.HideRow(5);  // Row 6 (0-based index 5)
            cells.HideRow(8);  // Row 9 (0-based index 8)

            // Überprüfen und anzeigen des IsHidden-Status für jede Zeile
            for (int i = 0; i < 10; i++)
            {
                bool isHidden = cells.Rows[i].IsHidden;
                Console.WriteLine($"Row {i + 1} is hidden: {isHidden}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RowHiddenDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


