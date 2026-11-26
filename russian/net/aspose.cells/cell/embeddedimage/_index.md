---
title: "Cell.EmbeddedImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает и задает встроенное изображение в ячейке"
type: docs
url: /ru/net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Получает и задает встроенное изображение в ячейке.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellPropertyEmbeddedImageDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте новую книгу и получите первый лист
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Выберите ячейку для хранения встроенного изображения
                Cell cell = worksheet.Cells["B2"];

                // Прозрачный PNG 1x1 пиксель (закодированный в Base64)
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // Преобразуйте строку Base64 в массив байтов
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // Установите встроенное изображение в ячейку
                cell.EmbeddedImage = imageBytes;

                // Получите встроенное изображение обратно из ячейки
                byte[] retrievedBytes = cell.EmbeddedImage;

                // Запишите полученное изображение в файл, чтобы проверить, что оно было сохранено корректно
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // Сохраните книгу (встроенное изображение хранится внутри .xlsx)
                string workbookPath = "EmbeddedImageDemo.xlsx";
                workbook.Save(workbookPath);
                Console.WriteLine($"Workbook saved to: {Path.GetFullPath(workbookPath)}");
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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


