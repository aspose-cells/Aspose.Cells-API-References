---
title: "ThreeDFormat.LightingDirection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает направление, из которого световое оборудование ориентировано относительно сцены"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/lightingdirection/
---
## ThreeDFormat.LightingDirection property

Получает и задает направление, из которого световая установка ориентирована относительно сцены.

```csharp
public LightRigDirectionType LightingDirection { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDirectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D Lighting Direction Demo";
            
            // Получите ThreeDFormat фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Установите начальные 3D‑свойства
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.Material = PresetMaterialType.Plastic;

            // Отобразить текущее направление освещения
            Console.WriteLine("Current LightingDirection: " + threeDFormat.LightingDirection);

            // Измените направление освещения и наблюдайте за эффектами
            threeDFormat.LightingDirection = LightRigDirectionType.TopLeft;
            Console.WriteLine("Changed LightingDirection to TopLeft");

            // Перейти к другому направлению
            threeDFormat.LightingDirection = LightRigDirectionType.BottomRight;
            Console.WriteLine("Changed LightingDirection to BottomRight");

            // Сохраните рабочую книгу, чтобы увидеть визуальные эффекты
            workbook.Save("ThreeDFormatLightingDirectionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [LightRigDirectionType](../../lightrigdirectiontype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


