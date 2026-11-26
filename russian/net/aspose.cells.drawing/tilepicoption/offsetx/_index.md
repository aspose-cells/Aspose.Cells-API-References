---
title: "TilePicOption.OffsetX"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TilePicOption. Получает или задает смещение по оси X для мозаичной картинки"
type: docs
url: /ru/net/aspose.cells.drawing/tilepicoption/offsetx/
---
## TilePicOption.OffsetX property

Получает или задает смещение по оси X для изображения замощения.

```csharp
public double OffsetX { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TilePicOptionPropertyOffsetXDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму для демонстрации мозаики
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Настройте формат заливки для использования мозаичной картинки
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Создать и настроить TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Прочитайте начальное значение OffsetX
            Console.WriteLine("Current OffsetX value: " + tileOptions.OffsetX);

            // Установите новое смещение X для мозаичного шаблона
            tileOptions.OffsetX = 15.5;

            // Примените параметры мозаики к заливке формы
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Загрузите минимальное изображение 1×1 пиксель (красная точка)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Сохранить изменённую книгу
            workbook.Save("TilePicOptionPropertyOffsetXDemo.xlsx");
        }
    }
}
```

### См. также

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


