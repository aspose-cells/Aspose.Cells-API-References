---
title: "MsoFormatPicture.Gamma"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFormatPicture. Представляет гамму изображения"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/gamma/
---
## MsoFormatPicture.Gamma property

Представляет гамму изображения.

```csharp
public double Gamma { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyGammaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте изображение в лист (используя пример пути к изображению)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Получить доступ к объекту MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Установите свойство Gamma
            formatPicture.Gamma = 1.5; // Demonstrating Gamma adjustment

            // Сохраните книгу
            workbook.Save("MsoFormatPictureGammaDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


