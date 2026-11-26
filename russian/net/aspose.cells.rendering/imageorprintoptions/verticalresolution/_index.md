---
title: "ImageOrPrintOptions.VerticalResolution"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает вертикальное разрешение генерируемых изображений в точках на дюйм"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/verticalresolution/
---
## ImageOrPrintOptions.VerticalResolution property

Получает или задает вертикальное разрешение для сгенерированных изображений в точках на дюйм.

```csharp
public int VerticalResolution { get; set; }
```

### Примечания

Значение по умолчанию — 96.

Настройка [`HorizontalResolution`](../horizontalresolution/) и `VerticalResolution` влияет на ширину и высоту выходного изображения в пикселях.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyVerticalResolutionDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные и создайте диаграмму
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Создайте параметры изображения с определённым вертикальным разрешением
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.VerticalResolution = 300; // Setting vertical resolution to 300 DPI
            options.HorizontalResolution = 300; // For consistency, setting horizontal resolution too

            // Сохраните диаграмму как изображение с указанным разрешением
            chart.ToImage("output_chart.png", options);
            
            Console.WriteLine("Chart saved as image with vertical resolution of 300 DPI.");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


