---
title: "ImageOrPrintOptions.CustomPrintPageEventHandler"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Клиент может выполнять специальный вывод на принтер при печати каждой страницы, используя этот EventHandler"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/
---
## ImageOrPrintOptions.CustomPrintPageEventHandler property

Клиент может выполнять специальный вывод на принтер при печати каждой страницы с использованием этого EventHandler

```csharp
public PrintPageEventHandler CustomPrintPageEventHandler { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomPrintPageEventHandlerDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Sample Data for Printing";
            worksheet.Cells["A2"].Value = "This demonstrates printing options";

            try
            {
                // Создайте экземпляр ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Настройте параметры печати
                options.PrintWithStatusDialog = true;
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;

                // Отобразить текущие параметры печати
                Console.WriteLine($"PrintWithStatusDialog: {options.PrintWithStatusDialog}");
                Console.WriteLine($"HorizontalResolution: {options.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {options.VerticalResolution}");

                // Создать SheetRender для демонстрации печати
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Отобразить в изображение для демонстрации печати
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Rendering completed successfully.");
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


