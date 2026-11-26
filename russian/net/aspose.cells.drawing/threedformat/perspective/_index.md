---
title: "ThreeDFormat.Perspective"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает угол, под которым можно просматривать объект ThreeDFormat"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/perspective/
---
## ThreeDFormat.Perspective property

Получает и задает угол, под которым можно просматривать объект ThreeDFormat.

```csharp
public double Perspective { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 200, 100);
            
            // Получить 3D-формат фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Отобразить текущее значение перспективы
            Console.WriteLine("Current Perspective value: " + threeDFormat.Perspective);

            // Установить новое значение перспективы (от 0 до 120 градусов)
            threeDFormat.Perspective = 45;
            Console.WriteLine("Perspective set to: " + threeDFormat.Perspective);

            // Применить другие 3D‑эффекты для лучшей визуализации изменения перспективы
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Сохраните книгу, чтобы увидеть эффекты
            workbook.Save("ThreeDFormatPerspectiveDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


