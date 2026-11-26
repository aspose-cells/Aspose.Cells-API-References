---
title: "Перечисление SvgEmbeddedFontType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.SvgEmbeddedFontType. Представляет тип встроенного шрифта в SVG‑изображении"
type: docs
url: /ru/net/aspose.cells.rendering/svgembeddedfonttype/
---
## SvgEmbeddedFontType enumeration

Представляет тип встроенного шрифта в изображении SVG.

```csharp
public enum SvgEmbeddedFontType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Не встраивать шрифт. |
| Woff | `1` | Встроить шрифт WOFF. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Настроить параметры изображения SVG
            SvgImageOptions svgOptions = new SvgImageOptions
            {
                EmbeddedFontType = SvgEmbeddedFontType.Woff,
                FitToViewPort = true,
                CssPrefix = "chart-prefix"
            };

            // Сохранить диаграмму в формате SVG с внедрённым шрифтом WOFF
            chart.ToImage("output_chart.svg", svgOptions);

            Console.WriteLine("SVG with embedded WOFF font generated successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


