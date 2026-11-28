---
title: "CellsColor.Color"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsColor özelliği. RGB rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

RGB rengi alır ve ayarlar.

```csharp
public Color Color { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralık oluşturun ve renkli kenarlıklar ayarlayın
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);

            // Bir hücredeki kenarlık ayarlarını doğrulayın
            Cell cell = worksheet.Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            // Çalışma kitabını kaydedin
            workbook.Save("CellsColorPropertyColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


