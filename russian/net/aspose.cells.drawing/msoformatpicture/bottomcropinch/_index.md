---
title: "MsoFormatPicture.BottomCropInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MsoFormatPicture property. Представляет положение нижней части прямоугольника обрезки, выраженное в дюймах"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/bottomcropinch/
---
## MsoFormatPicture.BottomCropInch property

Представляет расположение нижней части прямоугольника обрезки, в дюймах.

```csharp
public double BottomCropInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBottomCropInchDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить изображение на лист (используя путь-заполнитель)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Получить доступ к объекту MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Установить свойство BottomCropInch и продемонстрировать его использование
            formatPicture.BottomCropInch = 0.3;
            formatPicture.TopCropInch = 0.2;
            
            // Сохраните книгу
            workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


