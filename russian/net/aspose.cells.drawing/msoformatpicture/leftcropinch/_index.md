---
title: "MsoFormatPicture.LeftCropInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFormatPicture. Представляет положение левой стороны области обрезки, выраженное в дюймах"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

Представляет расположение левой стороны прямоугольника обрезки, в дюймах.

```csharp
public double LeftCropInch { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropInchDemo
    {
        public static void Run()
        {
            // Создать книгу
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // Загрузить данные изображения
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // Добавить изображение в лист
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // Установите и получите свойство LeftCropInch
            picture.FormatPicture.LeftCropInch = 0.5;
            double leftCropValue = picture.FormatPicture.LeftCropInch;

            Console.WriteLine($"Left crop value in inches: {leftCropValue}");

            // Сохраните книгу
            workbook.Save("LeftCropInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


