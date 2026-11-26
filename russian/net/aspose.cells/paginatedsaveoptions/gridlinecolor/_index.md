---
title: "PaginatedSaveOptions.GridlineColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Получает или задает цвет линий сетки"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

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
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Создайте параметры сохранения PDF
                PdfSaveOptions options = new PdfSaveOptions();

                // Отобразите значение цвета линий сетки по умолчанию
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // Установите новый цвет линий сетки
                options.GridlineColor = Color.Red;

                // Отобразите обновлённое значение цвета линий сетки
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // Сохраните книгу с настройкой цвета линий сетки
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


