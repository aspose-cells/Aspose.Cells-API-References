---
title: "Shape.FormatPicture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает параметры формата изображения"
type: docs
url: /ru/net/aspose.cells.drawing/shape/formatpicture/
---
## Shape.FormatPicture property

Получает и задает параметры формата изображения.

```csharp
public MsoFormatPicture FormatPicture { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFormatPictureDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Получить доступ к свойству FormatPicture фигуры
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;
            
            // Изменить свойства формата изображения
            msoFormatPicture.Brightness = 0.5f;
            msoFormatPicture.Contrast = 0.7f;
            msoFormatPicture.Transparency = 0.3f;
            
            // Сохраните книгу
            workbook.Save("ShapePropertyFormatPictureDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../../msoformatpicture/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


