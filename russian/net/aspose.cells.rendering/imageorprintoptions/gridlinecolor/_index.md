---
title: "ImageOrPrintOptions.GridlineColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает цвет линий сетки"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

Получает или задает цвет линий сетки.

```csharp
public Color GridlineColor { get; set; }
```

### Примечания

Он будет игнорировать настройки цвета линий сетки в исходном файле.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Поместите некоторые примерные данные, чтобы лист имел содержимое
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // Создайте экземпляр ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Отобразить текущее значение GridlineColor (только для чтения или чтение/запись)
                // Тип свойства предполагается System.Drawing.Color
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // При желании отобразите лист в виде изображения, чтобы увидеть эффект цвета линий сетки по умолчанию
                // (Не требуется менять значение; мы лишь демонстрируем использование.)
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // Сохраните книгу (необязательно)
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


