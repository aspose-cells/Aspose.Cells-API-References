---
title: "Класс ThreeDFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ThreeDFormat. Представляет трехмерное форматирование фигур"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/
---
## ThreeDFormat class

Представляет трехмерное форматирование фигуры.

```csharp
public class ThreeDFormat
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BottomBevelHeight](../../aspose.cells.drawing/threedformat/bottombevelheight/) { get; set; } | Получает и задает высоту нижнего скоса, или насколько глубоко он применяется к фигуре. В единицах точек. |
| [BottomBevelType](../../aspose.cells.drawing/threedformat/bottombeveltype/) { get; set; } | Получает и задает тип нижнего скоса, или насколько глубоко он применяется к фигуре. В единицах точек. |
| [BottomBevelWidth](../../aspose.cells.drawing/threedformat/bottombevelwidth/) { get; set; } | Получает и задает ширину нижнего скоса, или насколько глубоко он применяется к фигуре. В единицах точек. |
| [ContourColor](../../aspose.cells.drawing/threedformat/contourcolor/) { get; set; } | Получает и задает цвет контура фигуры. |
| [ContourWidth](../../aspose.cells.drawing/threedformat/contourwidth/) { get; set; } | Получает и задает ширину контура фигуры, в единицах точек. |
| [ExtrusionColor](../../aspose.cells.drawing/threedformat/extrusioncolor/) { get; set; } | Получает цвет экструдирования фигуры. |
| [ExtrusionHeight](../../aspose.cells.drawing/threedformat/extrusionheight/) { get; set; } | Получает и задает высоту экструдирования, применяемую к фигуре, в единицах точек. |
| [LightAngle](../../aspose.cells.drawing/threedformat/lightangle/) { get; set; } | Получает и задает угол света экструдирования. |
| [Lighting](../../aspose.cells.drawing/threedformat/lighting/) { get; set; } | Получает и задает тип световой установки. |
| [LightingDirection](../../aspose.cells.drawing/threedformat/lightingdirection/) { get; set; } | Получает и задает направление, из которого световая установка ориентирована относительно сцены. |
| [Material](../../aspose.cells.drawing/threedformat/material/) { get; set; } | Представляет предустановленный материал, который комбинируется со свойствами освещения, чтобы создать окончательный внешний вид фигуры. |
| [Perspective](../../aspose.cells.drawing/threedformat/perspective/) { get; set; } | Получает и задает угол, под которым можно просматривать объект ThreeDFormat. |
| [PresetCameraType](../../aspose.cells.drawing/threedformat/presetcameratype/) { get; set; } | Получает и задает тип предустановленной камеры экструдирования. |
| [RotationX](../../aspose.cells.drawing/threedformat/rotationx/) { get; set; } | Получает и задает вращение экструдированной фигуры вокруг оси X в градусах. |
| [RotationY](../../aspose.cells.drawing/threedformat/rotationy/) { get; set; } | Получает и задает вращение экструдированной фигуры вокруг оси Y в градусах. |
| [RotationZ](../../aspose.cells.drawing/threedformat/rotationz/) { get; set; } | Получает и задает вращение экструдированной фигуры вокруг оси Z в градусах. |
| [TopBevelHeight](../../aspose.cells.drawing/threedformat/topbevelheight/) { get; set; } | Получает и задает высоту верхнего скоса, или насколько глубоко он применяется к фигуре. В единицах точек. |
| [TopBevelType](../../aspose.cells.drawing/threedformat/topbeveltype/) { get; set; } | Получает и задает тип верхней фаски, или насколько глубоко она применяется к фигуре. В единицах точек. |
| [TopBevelWidth](../../aspose.cells.drawing/threedformat/topbevelwidth/) { get; set; } | Получает и задает ширину верхней фаски, или насколько глубоко она применяется к фигуре. В единицах точек. |
| [Z](../../aspose.cells.drawing/threedformat/z/) { get; set; } | Определяет расстояние от земли для 3D‑формы. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/threedformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/threedformat/gethashcode/)() | Получает хеш‑код. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassThreeDFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 210, 210, 200, 200);
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.ExtrusionHeight = 20;

            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


