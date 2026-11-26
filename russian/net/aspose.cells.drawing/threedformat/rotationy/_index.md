---
title: "ThreeDFormat.RotationY"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает вращение выдавленной фигуры вокруг оси Y в градусах"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/rotationy/
---
## ThreeDFormat.RotationY property

Получает и задает вращение экструдированной фигуры вокруг оси Y в градусах.

```csharp
public double RotationY { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationYDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 100, 150, 150);
            shape.Text = "3D Rotation Demo";
            
            // Получите доступ к ThreeDFormat фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Отобразите текущее значение RotationY
            Console.WriteLine("Current RotationY value: " + threeDFormat.RotationY);

            // Установите новые значения RotationY и продемонстрируйте эффекты
            threeDFormat.RotationY = 15;
            Console.WriteLine("Shape rotated 15 degrees around Y-axis");

            // Примените некоторые другие 3D‑свойства, чтобы сделать эффект видимым
            threeDFormat.ExtrusionHeight = 5;
            threeDFormat.ContourWidth = 1;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Сохраните книгу, чтобы показать эффекты
            workbook.Save("ThreeDFormatRotationYDemo.xlsx");

            // Измените вращение снова и сохраните другую версию
            threeDFormat.RotationY = 45;
            workbook.Save("ThreeDFormatRotationYDemo_45degrees.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


