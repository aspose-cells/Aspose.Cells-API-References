---
title: "MsoFormatPicture.Brightness"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFormatPicture. Представляет изменение яркости изображения в процентах"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/brightness/
---
## MsoFormatPicture.Brightness property

Представляет изменение яркости изображения в процентах.

```csharp
public double Brightness { get; set; }
```

### Примечания

Значение находится в диапазоне от -100% до 100%. Работает так же, как в Excel 2007 и более новых версиях.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBrightnessDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[pictureIndex];

            // Установить и получить яркость
            picture.FormatPicture.Brightness = 30;
            Console.WriteLine("Picture brightness: " + picture.FormatPicture.Brightness);

            // Изменить яркость
            picture.FormatPicture.Brightness = 70;
            Console.WriteLine("Updated brightness: " + picture.FormatPicture.Brightness);
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


