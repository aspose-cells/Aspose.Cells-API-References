---
title: "SvgImageOptions.CssPrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SvgImageOptions. Получает и задаёт префикс имени css в svg, значение по умолчанию — пустая строка"
type: docs
url: /ru/net/aspose.cells.rendering/svgimageoptions/cssprefix/
---
## SvgImageOptions.CssPrefix property

Получает и задает префикс имени CSS в SVG, значение по умолчанию — пустая строка.

```csharp
public string CssPrefix { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyCssPrefixDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue(2019);
            worksheet.Cells["A3"].PutValue(2020);
            worksheet.Cells["A4"].PutValue(2021);
            worksheet.Cells["A5"].PutValue(2022);

            worksheet.Cells["B2"].PutValue(4500);
            worksheet.Cells["B3"].PutValue(4900);
            worksheet.Cells["B4"].PutValue(5200);
            worksheet.Cells["B5"].PutValue(6100);

            // Создать линейный график
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B5", true);

            // Создать параметры изображения SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Отобразить текущий префикс CSS
            Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);

            // Установить новый префикс CSS
            svgOptions.CssPrefix = "chart-prefix-";

            // Продемонстрировать генерацию SVG с пользовательским префиксом CSS
            string outputPath = "output_chart.svg";
            chart.ToImage(outputPath, svgOptions);

            Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
        }
    }
}
```

### См. также

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


