---
title: "CellsColor.Transparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsColor özelliği. Şeffaflığı 0.0 opak'tan 1.0 tamamen şeffaf'a kadar bir değer olarak alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cellscolor/transparency/
---
## CellsColor.Transparency property

Şeffaflığı 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır ve ayarlar.

```csharp
public double Transparency { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyTransparencyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Color = Color.FromArgb(128, 255, 0, 0); // Semi-transparent red
            cellsColor.Transparency = 0.5; // Set transparency to 50%

            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;

            worksheet.Cells["A1"].PutValue("50% transparent red background");
            worksheet.Cells["A1"].SetStyle(style);

            workbook.Save("TransparencyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


