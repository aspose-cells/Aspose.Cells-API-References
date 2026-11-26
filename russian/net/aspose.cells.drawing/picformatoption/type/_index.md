---
title: "PicFormatOption.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PicFormatOption. Получает или задает тип заливки изображения"
type: docs
url: /ru/net/aspose.cells.drawing/picformatoption/type/
---
## PicFormatOption.Type property

Получает или задаёт тип заливки изображения.

```csharp
public FillPictureType Type { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте простое BMP-изображение размером 1×1 пиксель
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // Добавить изображение в лист
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes));
            Picture picture = worksheet.Pictures[pictureIndex];

            // Установите позицию и размер изображения
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 5;
            picture.LowerRightColumn = 5;

            try
            {
                // Получите PicFormatOption из текстурной заливки изображения
                PicFormatOption picFormat = picture.Fill.TextureFill.PicFormatOption;

                // Отобразить текущее значение Type
                Console.WriteLine("Current Type: " + picFormat.Type);

                // Установите различные значения Type и отобразите их
                picFormat.Type = FillPictureType.Stretch;
                Console.WriteLine("Type set to Stretch: " + picFormat.Type);

                picFormat.Type = FillPictureType.Stack;
                Console.WriteLine("Type set to Stack: " + picFormat.Type);

                picFormat.Type = FillPictureType.StackAndScale;
                Console.WriteLine("Type set to StackAndScale: " + picFormat.Type);

                // Сохраните книгу
                workbook.Save("PicFormatOptionTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [FillPictureType](../../fillpicturetype/)
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


