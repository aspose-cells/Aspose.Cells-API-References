---
title: "Shape.RelativeToOriginalPictureSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, относится ли фигура к исходному размеру изображения"
type: docs
url: /ru/net/aspose.cells.drawing/shape/relativetooriginalpicturesize/
---
## Shape.RelativeToOriginalPictureSize property

Указывает, является ли фигура относительной к исходному размеру изображения.

```csharp
public bool RelativeToOriginalPictureSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRelativeToOriginalPictureSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Получить доступ к свойствам фигуры — Picture уже является Shape, кастовать не требуется
            Shape shape = picture;

            // Продемонстрировать свойство RelativeToOriginalPictureSize
            Console.WriteLine("Original RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
            
            // Изменить свойство
            shape.RelativeToOriginalPictureSize = !shape.RelativeToOriginalPictureSize;
            Console.WriteLine("Modified RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


