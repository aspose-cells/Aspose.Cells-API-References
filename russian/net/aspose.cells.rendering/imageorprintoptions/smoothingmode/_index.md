---
title: "ImageOrPrintOptions.SmoothingMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Указывает, применяется ли сглаживание (антиалиасинг) к линиям и кривым и к краям заполненных областей. Значение по умолчанию — SmoothingMode.None"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

Указывает, применяется ли сглаживание (антиалиасинг) к линиям и кривым и к краям заполненных областей. Значение по умолчанию — SmoothingMode.None

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySmoothingModeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Создайте экземпляр ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Отобразить некоторые из доступных свойств
                Console.WriteLine("HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("ImageType: " + options.ImageType);

                // Создайте SheetRender, чтобы продемонстрировать свойство
                SheetRender renderer = new SheetRender(worksheet, options);

                // Отрисуйте в поток памяти, чтобы продемонстрировать функциональность
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Sheet rendered successfully");
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Сохраните книгу
                workbook.Save("ImageOrPrintOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


