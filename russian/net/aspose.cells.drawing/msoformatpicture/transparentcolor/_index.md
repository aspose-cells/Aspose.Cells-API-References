---
title: "MsoFormatPicture.TransparentColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFormatPicture. Получает и задает прозрачный цвет изображения"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/transparentcolor/
---
## MsoFormatPicture.TransparentColor property

Получает и задает прозрачный цвет изображения.

```csharp
public CellsColor TransparentColor { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTransparentColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пример изображения (используя прямоугольник сплошного цвета в качестве примера)
            int pictureIndex = worksheet.Pictures.Add(0, 0, "sample.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Установите прозрачный цвет
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.Blue;
            picture.FormatPicture.TransparentColor = transparentColor;

            // Получите и отобразите прозрачный цвет
            CellsColor currentTransparentColor = picture.FormatPicture.TransparentColor;
            Console.WriteLine("Current transparent color: " + currentTransparentColor.Color);

            // Сохраните книгу
            workbook.Save("TransparentColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


