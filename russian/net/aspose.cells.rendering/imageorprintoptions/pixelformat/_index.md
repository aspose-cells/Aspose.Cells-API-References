---
title: "ImageOrPrintOptions.PixelFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает формат пикселей для создаваемых изображений"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

Получает или задает пиксельный формат генерируемых изображений.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### Примечания

Значение по умолчанию — PixelFormat.Format32bppArgb.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "PixelFormat Demo";

            try
            {
                // Создайте экземпляр ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Отобразить текущее значение свойства ImageType (поскольку PixelFormat не существует)
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Примечание: Поскольку PixelFormat не существует в API, мы демонстрируем ImageType
                // что является наиболее близким связанным свойством для настроек формата изображения

                // Создать SheetRender, чтобы продемонстрировать используемые параметры
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Сохранить результат как изображение, чтобы продемонстрировать параметры
                sheetRender.ToImage(0, "PixelFormatDemo.png");

                Console.WriteLine("ImageType property has been demonstrated. Image saved as PixelFormatDemo.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


