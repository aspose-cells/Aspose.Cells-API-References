---
title: "BorderCollection.DiagonalStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BorderCollection egenskap. Hämtar eller anger stilen för diagonala linjer"
type: docs
url: /sv/net/aspose.cells/bordercollection/diagonalstyle/
---
## BorderCollection.DiagonalStyle property

Hämtar eller anger style för diagonala linjer.

```csharp
public CellBorderType DiagonalStyle { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta en cell och dess stil
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Ange diagonala border-egenskaper
            style.Borders.DiagonalStyle = CellBorderType.Thin;
            style.Borders.DiagonalColor = Color.Red;
            
            // Tillämpa stilen på cellen
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


