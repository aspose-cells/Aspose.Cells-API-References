---
title: "CellRichValue.Image"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellRichValue. Получает данные изображения ячейки"
type: docs
url: /ru/net/aspose.cells/cellrichvalue/image/
---
## CellRichValue.Image property

Получает данные изображения ячейки.

```csharp
public virtual byte[] Image { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class CellRichValuePropertyImageDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение в лист
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Получить сложное значение ячейки, содержащее изображение
            Cell cell = worksheet.Cells[0, 0];
            cell.PutValue("test data");
            cell.EmbeddedImage = picture.Data;

            // Получить доступ к сложному значению
            CellRichValue richValue = cell.GetRichValue();

            // Отобразить свойства изображения
            Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
            Console.WriteLine("Alt text: " + richValue.AltText);

            // Установить новый альтернативный текст для изображения
            richValue.AltText = "Sample product image";

            // Сохраните книгу
            workbook.Save("CellRichValueImageDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


