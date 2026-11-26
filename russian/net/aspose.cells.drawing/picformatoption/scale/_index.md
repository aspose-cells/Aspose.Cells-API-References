---
title: "PicFormatOption.Scale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PicFormatOption. Возвращает или задает, с чем изображение складывается и масштабируется"
type: docs
url: /ru/net/aspose.cells.drawing/picformatoption/scale/
---
## PicFormatOption.Scale property

Получает или задаёт количество, с которым изображение складывается и масштабируется.

```csharp
public double Scale { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO; // Added to resolve Stream-related issues

    public class PicFormatOptionPropertyScaleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте массив байтов BMP‑изображения размером 1×1 пиксель
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // Добавьте изображение в лист с помощью MemoryStream
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes)); // Fixed Stream conversion
            Picture picture = worksheet.Pictures[pictureIndex];

            // Настройте позицию и размер изображения
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 1;
            picture.LowerRightColumn = 1;

            // Получите текстурную заливку через свойство FillFormat
            TextureFill textureFill = picture.Fill.TextureFill; // Fixed cast error
            textureFill.PicFormatOption.Type = FillPictureType.Stack;

            // Отобразите и измените свойство Scale
            PicFormatOption picFormat = textureFill.PicFormatOption;
            Console.WriteLine("Current Scale value: " + picFormat.Scale);
            picFormat.Scale = 0.5;
            Console.WriteLine("Modified Scale value: " + picFormat.Scale);

            // Увеличьте размеры ячейки, чтобы визуализировать эффект
            worksheet.Cells.SetRowHeight(0, 100);
            worksheet.Cells.SetColumnWidth(0, 20);

            // Сохраните книгу
            workbook.Save("PropertyScaleDemo.xlsx");
        }
    }
}
```

### См. также

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


