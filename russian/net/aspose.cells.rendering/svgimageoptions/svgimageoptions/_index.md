---
title: "SvgImageOptions.SvgImageOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор SvgImageOptions. Ctor"
type: docs
url: /ru/net/aspose.cells.rendering/svgimageoptions/svgimageoptions/
---
## SvgImageOptions constructor

Конструктор.

```csharp
public SvgImageOptions()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Month");
            worksheet.Cells["A2"].PutValue("Jan");
            worksheet.Cells["A3"].PutValue("Feb");
            worksheet.Cells["A4"].PutValue("Mar");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(210);
            worksheet.Cells["B4"].PutValue(150);

            // Создать линейный график
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Создать SvgImageOptions с помощью конструктора
                SvgImageOptions svgOptions = new SvgImageOptions();

                // Настройте параметры рендеринга SVG
                svgOptions.ImageType = ImageType.Svg; // Explicitly set to SVG
                svgOptions.FitToViewPort = true;
                svgOptions.CssPrefix = "chart-prefix";
                svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

                // Сохранить график как SVG с указанными параметрами
                chart.ToImage("output_chart.svg", svgOptions);

                Console.WriteLine("SVG image saved successfully with specified options.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error generating SVG: {ex.Message}");
            }

            // Сохранить книгу, чтобы продемонстрировать исходные данные
            workbook.Save("SvgImageOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


