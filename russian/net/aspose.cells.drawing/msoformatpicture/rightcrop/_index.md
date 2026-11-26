---
title: "MsoFormatPicture.RightCrop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MsoFormatPicture property. Представляет положение правой стороны прямоугольника обрезки, выраженное в виде отношения к ширине изображения"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/rightcrop/
---
## MsoFormatPicture.RightCrop property

Представляет расположение правой стороны прямоугольника обрезки, выраженное как отношение к ширине изображения.

```csharp
public double RightCrop { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyRightCropDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Получить MsoFormatPicture изображения
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;

            // Отобразить текущее значение RightCrop
            Console.WriteLine("Current RightCrop value: " + msoFormatPicture.RightCrop);

            // Установить новое значение RightCrop (0.2 означает обрезку 20% справа)
            msoFormatPicture.RightCrop = 0.2;
            Console.WriteLine("New RightCrop value set to: " + msoFormatPicture.RightCrop);

            // Сохранить рабочую книгу, чтобы увидеть эффект
            workbook.Save("RightCropDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


