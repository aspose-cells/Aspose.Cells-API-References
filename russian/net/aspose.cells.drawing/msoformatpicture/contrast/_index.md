---
title: "MsoFormatPicture.Contrast"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFormatPicture. Представляет изменение контраста изображения в процентах"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/contrast/
---
## MsoFormatPicture.Contrast property

Представляет изменение контрастности изображения в процентах.

```csharp
public double Contrast { get; set; }
```

### Примечания

Значение находится в диапазоне от -100% до 100%. Работает так же, как в Excel 2007 и более новых версиях.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyContrastDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            var picture = worksheet.Pictures[pictureIndex];

            // Установите и получите значение контраста
            picture.FormatPicture.Contrast = 50;
            Console.WriteLine("Current contrast: " + picture.FormatPicture.Contrast);

            // Измените контраст
            picture.FormatPicture.Contrast = 75;
            Console.WriteLine("Modified contrast: " + picture.FormatPicture.Contrast);

            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


