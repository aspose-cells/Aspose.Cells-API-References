---
title: "ImageOrPrintOptions.GridlineType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает тип линий сетки"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/gridlinetype/
---
## ImageOrPrintOptions.GridlineType property

Получает или задает тип линий сетки.

```csharp
public GridlineType GridlineType { get; set; }
```

### Примечания

По умолчанию тип Dotted.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // Создайте новую рабочую книгу и заполните её примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Book");
            worksheet.Cells["B2"].PutValue("$19.99");
            worksheet.Cells["A3"].PutValue("Pen");
            worksheet.Cells["B3"].PutValue("$2.99");

            // Создайте экземпляр ImageOrPrintOptions
            ImageOrPrintOptions imageOptions = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png,
                GridlineType = GridlineType.Dotted // Use valid enum value
            };

            // Отобразите текущий тип линий сетки
            Console.WriteLine("Initial GridlineType: " + imageOptions.GridlineType);

            // Отрендерьте лист с начальным типом линий сетки
            SheetRender solidLineRenderer = new SheetRender(worksheet, imageOptions);
            solidLineRenderer.ToImage(0, "SolidGridlines.png");

            // Измените тип линий сетки и отрендерьте снова
            imageOptions.GridlineType = GridlineType.Hair; // Use valid enum value
            Console.WriteLine("\nModified GridlineType: " + imageOptions.GridlineType);

            SheetRender dashedLineRenderer = new SheetRender(worksheet, imageOptions);
            dashedLineRenderer.ToImage(0, "DashedGridlines.png");

            Console.WriteLine("Generated images demonstrate different gridline styles.");
        }
    }
}
```

### См. также

* enum [GridlineType](../../../aspose.cells/gridlinetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


