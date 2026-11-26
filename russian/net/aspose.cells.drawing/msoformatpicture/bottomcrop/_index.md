---
title: "MsoFormatPicture.BottomCrop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MsoFormatPicture property. Представляет положение нижней части прямоугольника обрезки, выраженное в виде отношения к высоте изображения"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/bottomcrop/
---
## MsoFormatPicture.BottomCrop property

Представляет расположение нижней части прямоугольника обрезки, выраженное как отношение к высоте изображения.

```csharp
public double BottomCrop { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyBottomCropDemo
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

            // Отобразить текущее значение BottomCrop
            Console.WriteLine("Current BottomCrop value: " + msoFormatPicture.BottomCrop);

            // Установить новое значение BottomCrop (0.2 означает обрезку 20% снизу)
            msoFormatPicture.BottomCrop = 0.2;
            Console.WriteLine("BottomCrop set to: " + msoFormatPicture.BottomCrop);

            // Установить другие значения обрезки для демонстрации эффекта
            msoFormatPicture.TopCrop = 0.1;
            msoFormatPicture.LeftCrop = 0.1;
            msoFormatPicture.RightCrop = 0.1;

            // Сохранить книгу, чтобы увидеть обрезанное изображение
            workbook.Save("MsoFormatPicturePropertyBottomCropDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


