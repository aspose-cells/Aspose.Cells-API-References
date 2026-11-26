---
title: "ExportObjectEvent.GetSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ExportObjectEvent. Получает объект для экспорта"
type: docs
url: /ru/net/aspose.cells/exportobjectevent/getsource/
---
## ExportObjectEvent.GetSource method

Получает объект для экспорта.

```csharp
public object GetSource()
```

### Возвращаемое значение

объект для экспорта.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventMethodGetSourceDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте изображение, чтобы продемонстрировать работу функции GetSource
            int pictureIndex = worksheet.Pictures.Add(1, 1, "sample.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            try
            {
                // Создайте пользовательский слушатель экспорта объектов
                HtmlSaveOptions saveOptions = new HtmlSaveOptions
                {
                    ExportObjectListener = new CustomExportObjectListener()
                };

                // Сохраните книгу, чтобы вызвать событие ExportObjectEvent
                using (Stream stream = new FileStream("GetSourceDemo.html", FileMode.Create))
                {
                    workbook.Save(stream, saveOptions);
                }

                Console.WriteLine("GetSource method demonstrated successfully. Check the output HTML file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetSource: {ex.Message}");
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Продемонстрировать метод GetSource
            object source = e.GetSource();

            if (source is Picture)
            {
                Console.WriteLine("GetSource returned a Picture object");
                return "custom-image-url.jpg";
            }

            return null;
        }
    }
}
```

### См. также

* class [ExportObjectEvent](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


