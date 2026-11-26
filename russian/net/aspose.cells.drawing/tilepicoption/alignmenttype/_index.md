---
title: "TilePicOption.AlignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "TilePicOption свойство. Получает или задает выравнивание для плитки"
type: docs
url: /ru/net/aspose.cells.drawing/tilepicoption/alignmenttype/
---
## TilePicOption.AlignmentType property

Получает или задает выравнивание для замощения.

```csharp
public RectangleAlignmentType AlignmentType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму для демонстрации мозаики
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 300);

            // Настройте формат заливки для использования мозаичной картинки
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Создать и настроить TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Отобразить начальное значение AlignmentType
            Console.WriteLine("Current AlignmentType: " + tileOptions.AlignmentType);

            // Установить выравнивание в TopRight
            tileOptions.AlignmentType = RectangleAlignmentType.TopRight;
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;

            // Примените параметры мозаики к заливке формы
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Загрузить пример изображения (красная точка 1x1 пиксель)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Сохранить изменённую книгу
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo.xlsx");

            // Изменить выравнивание на BottomLeft и сохранить другую версию
            tileOptions.AlignmentType = RectangleAlignmentType.BottomLeft;
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo_BottomLeft.xlsx");
        }
    }
}
```

### См. также

* enum [RectangleAlignmentType](../../rectanglealignmenttype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


