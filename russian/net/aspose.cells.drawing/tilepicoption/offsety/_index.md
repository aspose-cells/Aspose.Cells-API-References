---
title: "TilePicOption.OffsetY"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TilePicOption. Получает или задает смещение по оси Y для мозаичной картинки"
type: docs
url: /ru/net/aspose.cells.drawing/tilepicoption/offsety/
---
## TilePicOption.OffsetY property

Получает или задает смещение по оси Y для изображения замощения.

```csharp
public double OffsetY { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyOffsetYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            string imagePath = CreateTempImage();

            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 0, 0, 300, 200);
            FillFormat fill = shape.Fill;
            fill.FillType = FillType.Texture;

            byte[] pictureData = File.ReadAllBytes(imagePath);
            fill.TextureFill.ImageData = pictureData; // Changed from .Picture to .ImageData

            TilePicOption tilePicOption = fill.TextureFill.TilePicOption;

            Console.WriteLine("Current OffsetY value: " + tilePicOption.OffsetY);

            tilePicOption.OffsetY = 20;

            workbook.Save("PropertyOffsetYDemo.xlsx");

            File.Delete(imagePath);
        }

        private static string CreateTempImage()
        {
            // Base64‑закодированный PNG размером 100×100 светло‑голубого цвета с темно‑синей окружностью
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAABWSURBVHhe7cEBAQAAAIIg/69uSEABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADgNwRkAAH7nKfTAAAAAElFTkSuQmCC";
            byte[] imageBytes = Convert.FromBase64String(base64Image);
            string tempFile = Path.GetTempFileName() + ".png";
            File.WriteAllBytes(tempFile, imageBytes);
            return tempFile;
        }
    }
}
```

### См. также

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


