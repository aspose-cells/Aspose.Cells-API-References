---
title: "Style.Borders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar BorderCollection för stilen"
type: docs
url: /sv/net/aspose.cells/style/borders/
---
## Style.Borders property

Hämtar [`BorderCollection`](../../bordercollection/) för stilen.

```csharp
public BorderCollection Borders { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBordersDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta cellen och dess stil
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Ställ in olika kantstilar
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            
            // Tillämpa stilen på cellen
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("BorderStylesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


