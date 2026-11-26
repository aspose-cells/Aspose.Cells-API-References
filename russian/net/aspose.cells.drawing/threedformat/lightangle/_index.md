---
title: "ThreeDFormat.LightAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает угол освещения экструдирования"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/lightangle/
---
## ThreeDFormat.LightAngle property

Получает и задает угол света экструдирования.

```csharp
public double LightAngle { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D Format Demo";
            
            // Получите доступ к ThreeDFormat фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Отобразить текущее значение LightAngle
            Console.WriteLine("Current LightAngle value: " + threeDFormat.LightAngle);

            // Установить новое значение LightAngle (от 0 до 359,9 градусов)
            threeDFormat.LightAngle = 45;
            Console.WriteLine("New LightAngle value: " + threeDFormat.LightAngle);

            // Настроить другие 3D‑свойства, чтобы увидеть эффект LightAngle
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Сохраните книгу, чтобы увидеть эффекты
            workbook.Save("ThreeDFormatLightAngleDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


