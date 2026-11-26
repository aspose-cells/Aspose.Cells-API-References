---
title: "ThreeDFormat.Lighting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает тип светового оборудования"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/lighting/
---
## ThreeDFormat.Lighting property

Получает и задает тип световой установки.

```csharp
public LightRigType Lighting { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 200);
            shape.Text = "3D Lighting Demo";
            
            // Получите ThreeDFormat фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Отобразить текущее значение освещения
            Console.WriteLine("Current Lighting value: " + threeDFormat.Lighting);

            // Установите разные типы освещения и наблюдайте за эффектами
            threeDFormat.Lighting = LightRigType.BrightRoom;
            Console.WriteLine("Changed to BrightRoom lighting");

            // Примените некоторые другие 3D‑свойства, чтобы лучше увидеть эффект освещения
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;

            // Сохранить с первым типом освещения
            workbook.Save("BrightRoomLighting.xlsx");

            // Перейти к другому типу освещения
            threeDFormat.Lighting = LightRigType.Sunset;
            Console.WriteLine("Changed to Sunset lighting");
            workbook.Save("SunsetLighting.xlsx");

            // Перейти к третьему типу освещения
            threeDFormat.Lighting = LightRigType.ThreePoint;
            Console.WriteLine("Changed to ThreePoint lighting");
            workbook.Save("ThreePointLighting.xlsx");
        }
    }
}
```

### См. также

* enum [LightRigType](../../lightrigtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


