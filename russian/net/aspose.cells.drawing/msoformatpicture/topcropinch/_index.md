---
title: "MsoFormatPicture.TopCropInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFormatPicture. Представляет расположение верхней части прямоугольника обрезки, выраженное в дюймах"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/topcropinch/
---
## MsoFormatPicture.TopCropInch property

Представляет расположение верхней части прямоугольника обрезки, в дюймах.

```csharp
public double TopCropInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте изображение (замените реальным путем к файлу изображения)
            int pictureIndex = sheet.Pictures.Add(0, 0, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // Получите доступ и измените свойство TopCropInch
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.TopCropInch = 0.3; // Crop 0.3 inches from top
            format.BottomCropInch = 0.2; // Additional crop properties for context

            // Сохранить результат
            workbook.Save("TopCropInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


