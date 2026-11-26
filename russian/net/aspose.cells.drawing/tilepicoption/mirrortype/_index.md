---
title: "TilePicOption.MirrorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TilePicOption. Получает или задает тип отражения для мозаики"
type: docs
url: /ru/net/aspose.cells.drawing/tilepicoption/mirrortype/
---
## TilePicOption.MirrorType property

Получает или задает тип зеркального отражения для замощения.

```csharp
public MirrorType MirrorType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyMirrorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 500, 500, 500);

            // Загрузите примерные данные изображения (замените реальным путем к изображению)
            byte[] imageData = File.ReadAllBytes("sample.png");

            // Создайте и настройте экземпляр TilePicOption
            TilePicOption tileOptions = new TilePicOption();

            // Отобразить начальное значение MirrorType
            Console.WriteLine("Current MirrorType: " + tileOptions.MirrorType);

            // Настройте параметры мозаики
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;
            tileOptions.MirrorType = MirrorType.Both;

            // Применить конфигурацию плитки, используя правильные свойства
            shape.Fill.FillType = FillType.Texture;
            shape.Fill.ImageData = imageData;
            shape.Fill.TextureFill.TilePicOption = tileOptions;

            // Сохранить изменённую книгу
            workbook.Save("TilePicOptionMirrorTypeDemo.xlsx");

            Console.WriteLine("Updated MirrorType: " + tileOptions.MirrorType);
        }
    }
}
```

### См. также

* enum [MirrorType](../../mirrortype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


