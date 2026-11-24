---
title: "RowCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RowCollection‑Eigenschaft. Gibt ein Row‑Objekt anhand des angegebenen Zeilenindex zurück. Das Row‑Objekt des angegebenen Zeilenindex wird erstellt, falls es vorher nicht existiert."
type: docs
url: /de/net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

Gibt ein [`Row`](../../row/)‑Objekt anhand des angegebenen Zeilenindex zurück. Das Row‑Objekt des angegebenen Zeilenindex wird erstellt, falls es vorher nicht existiert.

```csharp
public Row this[int rowIndex] { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Standardbreite für Spalten festlegen
            cells.StandardWidth = 20.0;

            // Zugriff auf und Formatierung von Zeilen über die Item‑Eigenschaft
            for (int i = 0; i < 5; i++)
            {
                Row row = cells.Rows[i]; // Using Item property
                Style rowStyle = workbook.CreateStyle();
                rowStyle.Font.IsBold = true;
                rowStyle.Font.Color = System.Drawing.Color.Blue;
                row.ApplyStyle(rowStyle, new StyleFlag { Font = true });
                
                // Zugriff auf und Formatierung einer Zelle in der Zeile
                Cell cell = cells[i, i]; // Using Cells indexer instead of row[i]
                cell.PutValue($"Row {i}, Col {i}");
                Style cellStyle = workbook.CreateStyle();
                cellStyle.BackgroundColor = System.Drawing.Color.LightYellow;
                cell.SetStyle(cellStyle);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RowCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


