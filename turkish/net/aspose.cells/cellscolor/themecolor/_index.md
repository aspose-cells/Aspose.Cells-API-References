---
title: "CellsColor.ThemeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsColor özelliği. Tema rengini alır. Yalnızca tema rengi türü için geçerlidir"
type: docs
url: /tr/net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

Tema rengini alır. Yalnızca tema rengi türü için geçerlidir.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Bir CellsColor örneği oluştur
                CellsColor cellsColor = workbook.CreateCellsColor();

                // Bir tema rengi ayarlayın
                cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // ThemeColor özelliklerini gösterin
                Console.WriteLine("ThemeColor Type: " + cellsColor.ThemeColor.ColorType);
                Console.WriteLine("ThemeColor Tint: " + cellsColor.ThemeColor.Tint);

                // Rengi bir hücreye uygulayın
                Style style = workbook.CreateStyle();
                style.ForegroundColor = cellsColor.Color;
                style.Pattern = BackgroundType.Solid;

                worksheet.Cells["A1"].PutValue("Theme Color Example");
                worksheet.Cells["A1"].SetStyle(style);

                // Çalışma kitabını kaydedin
                workbook.Save("ThemeColorDemo.xlsx");
                Console.WriteLine("ThemeColor has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


