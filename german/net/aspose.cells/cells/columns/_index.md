---
title: "Cells.Columns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Ruft die Sammlung von Column-Objekten ab, die die einzelnen Spalten in diesem Arbeitsblatt darstellen"
type: docs
url: /de/net/aspose.cells/cells/columns/
---
## Cells.Columns property

Ruft die Sammlung von [`Column`](../../column/)-Objekten ab, die die einzelnen Spalten in diesem Arbeitsblatt darstellen.

```csharp
public ColumnCollection Columns { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyColumnsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Stil für Spalte 5 festlegen
            Style columnStyle = workbook.CreateStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 12;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { FontName = true, FontSize = true, FontBold = true });

            // Breite für Spalte 5 festlegen
            cells.Columns[5].Width = 20;

            // Daten in Spalte 5 festlegen, um den Stil zu demonstrieren
            for (int row = 0; row < 10; row++)
            {
                cells[row, 5].PutValue($"Row {row + 1}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ColumnsPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


