---
title: "ThreeDFormat.RotationX"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает вращение вытянутой фигуры вокруг оси x в градусах."
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/rotationx/
---
## ThreeDFormat.RotationX property

Получает и задает вращение экструдированной фигуры вокруг оси X в градусах.

```csharp
public double RotationX { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationXDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 2, 2, 200, 100, 100);
            
            // Получить 3D‑формат (не требуется "включать" 3D‑эффекты — достаточно установить свойства)
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Отобразить текущее значение RotationX
            Console.WriteLine("Current RotationX value: " + threeDFormat.RotationX);

            // Установить новое значение RotationX (вращение вокруг оси x в градусах)
            threeDFormat.RotationX = 45;
            Console.WriteLine("New RotationX value: " + threeDFormat.RotationX);

            // Установить другие 3D‑свойства, чтобы вращение стало видимым
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Сохраните книгу, чтобы увидеть эффекты
            workbook.Save("ThreeDFormatRotationXDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


