---
title: "FillFormat.TextureFill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Получает объект TextureFill"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/texturefill/
---
## FillFormat.TextureFill property

Получает объект `TextureFill`.

```csharp
public TextureFill TextureFill { get; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTextureFillDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму изображения
            string imagePath = Path.Combine("your_image_directory", "texture.png");
            int pictureIndex = worksheet.Pictures.Add(0, 0, imagePath);
            Shape picture = worksheet.Shapes[pictureIndex];

            // Установить свойства текстурного заполнения
            picture.Fill.TextureFill.ImageData = File.ReadAllBytes(imagePath);
            picture.Fill.TextureFill.IsTiling = true;
            picture.Fill.TextureFill.Scale = 0.5;

            // Сохраните книгу
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextureFill](../../texturefill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


