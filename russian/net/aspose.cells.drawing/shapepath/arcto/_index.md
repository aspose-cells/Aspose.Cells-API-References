---
title: "ShapePath.ArcTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapePath. Добавляет эллиптическую дугу к текущей фигуре. Начальная точка является конечной точкой текущей фигуры."
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

Добавляет эллиптическую дугу к текущей фигуре. Начальная точка является конечной точкой текущей фигуры.

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| wR | Single | Полуширина прямоугольной области эллипса, рисующей дугу (Unit: Pixel). |
| hR | Single | Полувысота прямоугольной области эллипса, рисующей дугу (Unit: Pixel). |
| stAng | Single | Начальный угол дуги, измеряемый в градусах по часовой стрелке от оси X (Unit: Degree). Этот угол определяет, какой угол вдоль предполагаемого кругового пути будет использоваться в качестве начальной позиции для рисования дуги. Этот начальный угол будет зафиксирован на последней известной позиции пера в пути ShapePath. Таким образом гарантируется непрерывный путь ShapePath. |
| swAng | Single | Угол разворота дуги. Этот угол определяет, насколько далеко по углу вдоль предполагаемого кругового пути будет продлена дуга. Расширение от начального угла всегда будет происходить по часовой стрелке вокруг предполагаемого круга. (Unit: Degree) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            //Создать новый путь формы
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);

            //Создать новый путь формы
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                        96.5f, -7.148871f,
                        130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                        182.24997f, 75.351f,
                        201, 120.517795f);
            shapePath1.MoveTo(150, 70);
            shapePath1.ArcTo(25, 25, 0, 270);

            Workbook workbook = new Workbook();

            //добавить свободную форму
            workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });

            // Сохранить результат
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


