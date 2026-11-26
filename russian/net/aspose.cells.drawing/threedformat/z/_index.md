---
title: "ThreeDFormat.Z"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Определяет расстояние от земли до 3D‑фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/z/
---
## ThreeDFormat.Z property

Определяет расстояние от земли для 3D‑формы.

```csharp
public double Z { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyZDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 100);
            
            // Получите доступ к ThreeDFormat фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Отобразить текущее значение Z (расстояние от земли)
            Console.WriteLine("Current Z value: " + threeDFormat.Z);

            // Установить новое значение Z, чтобы переместить фигуру дальше от земли
            threeDFormat.Z = 20;
            Console.WriteLine("New Z value: " + threeDFormat.Z);

            // Настроить другие 3D‑свойства, чтобы эффект стал видимым
            threeDFormat.ExtrusionHeight = 30;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Сохранить книгу, чтобы увидеть 3D‑эффект
            workbook.Save("ThreeDFormatPropertyZDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


