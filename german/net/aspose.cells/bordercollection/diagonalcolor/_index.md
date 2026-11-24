---
title: "BorderCollection.DiagonalColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BorderCollection‑Eigenschaft. Gibt die Farbe der diagonalen Linien zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/bordercollection/diagonalcolor/
---
## BorderCollection.DiagonalColor property

Liest oder setzt die Farbe der Diagonallinien.

```csharp
public Color DiagonalColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Border Demo");

            Style style = cell.GetStyle();
            
            // Festlegen diagonaler Rahmen‑Eigenschaften
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Thick;

            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


