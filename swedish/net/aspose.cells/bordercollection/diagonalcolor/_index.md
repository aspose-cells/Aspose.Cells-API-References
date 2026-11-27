---
title: "BorderCollection.DiagonalColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BorderCollection‑egenskap. Hämtar eller anger färgen på diagonala linjer"
type: docs
url: /sv/net/aspose.cells/bordercollection/diagonalcolor/
---
## BorderCollection.DiagonalColor property

Hämtar eller anger Color för diagonala linjer.

```csharp
public Color DiagonalColor { get; set; }
```

### Exempel

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
            
            // Inställning av diagonala kantegenskaper
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Thick;

            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


