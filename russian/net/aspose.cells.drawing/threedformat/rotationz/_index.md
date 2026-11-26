---
title: "ThreeDFormat.RotationZ"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает вращение вытянутой фигуры вокруг оси z в градусах."
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/rotationz/
---
## ThreeDFormat.RotationZ property

Получает и задает вращение экструдированной фигуры вокруг оси Z в градусах.

```csharp
public double RotationZ { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationZDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 0, 100, 150);
            shape.Text = "3D Rotation Demo";
            
            // Получите доступ к ThreeDFormat фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Отобразить текущее значение RotationZ
            Console.WriteLine("Current RotationZ value: " + threeDFormat.RotationZ);

            // Установить новые значения RotationZ и продемонстрировать эффекты
            threeDFormat.RotationZ = 45;
            Console.WriteLine("Shape rotated 45 degrees around Z-axis");

            // Применить другие 3D‑свойства, чтобы сделать вращение видимым
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Сохранить книгу с 3D‑эффектами
            workbook.Save("ThreeDFormatRotationZDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


