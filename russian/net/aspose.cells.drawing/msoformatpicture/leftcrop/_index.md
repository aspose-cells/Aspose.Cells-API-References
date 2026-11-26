---
title: "MsoFormatPicture.LeftCrop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFormatPicture. Представляет положение левой стороны прямоугольника обрезки, выраженное как отношение к ширине изображения"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/leftcrop/
---
## MsoFormatPicture.LeftCrop property

Представляет расположение левой стороны прямоугольника обрезки, выраженное как отношение к ширине изображения.

```csharp
public double LeftCrop { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropDemo
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

            // Установить свойство LeftCrop
            picture.FormatPicture.LeftCrop = 0.1;
            Console.WriteLine("LeftCrop set to: " + picture.FormatPicture.LeftCrop);

            // Получить и установить свойство LeftCropInch
            double leftCropInch = picture.FormatPicture.LeftCropInch;
            picture.FormatPicture.LeftCropInch = leftCropInch;
            Console.WriteLine("LeftCropInch value: " + leftCropInch);

            // Сохраните книгу
            workbook.Save("LeftCropDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


