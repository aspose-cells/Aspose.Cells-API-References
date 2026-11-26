---
title: "FillFormat.ImageData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Получает и задает данные изображения"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/imagedata/
---
## FillFormat.ImageData property

Получает и задает данные изображения картинки.

```csharp
public byte[] ImageData { get; set; }
```

### Примечания

Если формат заполнения не является пользовательским форматом текстуры, возвращает null.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyImageDataDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пример изображения в рабочий лист
            string imagePath = "example.png";
            worksheet.Pictures.Add(0, 0, imagePath);

            // Создать комментарий и задать данные изображения
            var comment = worksheet.Comments[worksheet.Comments.Add(2, 5)];
            byte[] imageData = File.ReadAllBytes(imagePath);
            comment.CommentShape.Fill.ImageData = imageData;

            // Сохранить книгу
            workbook.Save("FillFormatPropertyImageDataDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


