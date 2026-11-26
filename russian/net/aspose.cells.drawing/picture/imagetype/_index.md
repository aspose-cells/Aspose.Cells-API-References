---
title: "Picture.ImageType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. Возвращает формат изображения picture"
type: docs
url: /ru/net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

Получает формат изображения.

```csharp
public ImageType ImageType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyImageTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Вставить первое изображение (PNG)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            Console.WriteLine("Picture 1 is of type: " + pic1.ImageType);

            // Вставить второе изображение (JPEG)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            Console.WriteLine("Picture 2 is of type: " + pic2.ImageType);
        }
    }
}
```

### См. также

* enum [ImageType](../../imagetype/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


