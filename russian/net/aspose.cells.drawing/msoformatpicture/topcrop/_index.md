---
title: "MsoFormatPicture.TopCrop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFormatPicture. Представляет расположение верхней части прямоугольника обрезки, выраженное как отношение к высоте изображения"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/topcrop/
---
## MsoFormatPicture.TopCrop property

Представляет расположение верхней части прямоугольника обрезки, выраженное как отношение к высоте изображения.

```csharp
public double TopCrop { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить изображение на лист
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Установите свойство TopCrop
            picture.FormatPicture.TopCrop = -6;
            
            // Выведите значение TopCrop
            Console.WriteLine("Picture TopCrop value: " + picture.FormatPicture.TopCrop);
            
            // Сохраните книгу
            workbook.Save("TopCropDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


