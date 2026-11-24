---
title: "Cells.Rows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt die Sammlung von Row-Objekten zurück, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen"
type: docs
url: /de/net/aspose.cells/cells/rows/
---
## Cells.Rows property

Gibt die Sammlung von [`Row`](../../row/)‑Objekten zurück, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen.

```csharp
public RowCollection Rows { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRowsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze Spaltenbreite und Zeilenhöhe
            worksheet.Cells.SetColumnWidthPixel(0, 200);
            worksheet.Cells.Rows[0].Height = 50;
            
            // Greife auf Zeilen‑Eigenschaften über die Rows‑Sammlung zu
            Row row = worksheet.Cells.Rows[0];
            Console.WriteLine($"Row 0 height: {row.Height}");
            Console.WriteLine($"Is height matched: {row.IsHeightMatched}");
            
            // Ändere Zeilen‑Eigenschaften
            row.IsHeightMatched = true;
            row.Height = 60;
            
            // Überprüfe Änderungen
            Console.WriteLine($"Modified row 0 height: {worksheet.Cells.GetRowHeightPixel(0)}");
            Console.WriteLine($"Is height matched after change: {row.IsHeightMatched}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("CellsPropertyRowsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


