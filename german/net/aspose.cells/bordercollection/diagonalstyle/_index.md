---
title: "BorderCollection.DiagonalStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BorderCollection-Eigenschaft. Gibt den Stil der Diagonallinien zurück oder setzt ihn."
type: docs
url: /de/net/aspose.cells/bordercollection/diagonalstyle/
---
## BorderCollection.DiagonalStyle property

Liest oder setzt den Stil der Diagonallinien.

```csharp
public CellBorderType DiagonalStyle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hole eine Zelle und ihren Stil.
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Setze diagonale Rand-Eigenschaften.
            style.Borders.DiagonalStyle = CellBorderType.Thin;
            style.Borders.DiagonalColor = Color.Red;
            
            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


