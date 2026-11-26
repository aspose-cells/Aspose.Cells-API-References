---
title: "MsoFormatPicture.IsGray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFormatPicture. Указывает, должно ли изображение отображаться в градациях серого"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/isgray/
---
## MsoFormatPicture.IsGray property

Указывает, должно ли это изображение отображаться в градациях серого.

```csharp
public bool IsGray { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsGrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму изображения
            using (Stream imageStream = File.OpenRead("example.gif"))
            {
                Shape shape = worksheet.Shapes.AddPicture(0, 0, imageStream, 100, 100);
                
                // Установите свойства формата изображения
                shape.FormatPicture.Brightness = 90;
                shape.FormatPicture.Contrast = 90;
                shape.FormatPicture.IsGray = true;

                // Сохраните книгу
                workbook.Save("output.xlsx");
            }

            // Перезагрузите и проверьте свойства
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Brightness: " + loadedShape.FormatPicture.Brightness);
            Console.WriteLine("Contrast: " + loadedShape.FormatPicture.Contrast);
            Console.WriteLine("IsGray: " + loadedShape.FormatPicture.IsGray);
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


