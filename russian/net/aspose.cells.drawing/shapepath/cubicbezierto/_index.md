---
title: "ShapePath.CubicBezierTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ShapePath метод. Добавляет кубическую кривую Безье к текущей фигуре. Начальная точка является конечной точкой текущей фигуры. Единица измерения — пиксель"
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

Добавляет кубическую кривую Безье к текущей фигуре. Начальная точка является конечной точкой текущей фигуры. Единица измерения: пиксель.

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ctrX1 | Single | Координата x первой контрольной точки кривой (Единица: пиксель). |
| ctrY1 | Single | Координата y первой контрольной точки кривой (Единица: пиксель). |
| ctrX2 | Single | Координата x второй контрольной точки кривой (Единица: пиксель). |
| ctrY2 | Single | Координата y второй контрольной точки кривой (Единица: пиксель). |
| endX | Single | Координата x конечной точки кривой (Единица: пиксель). |
| endY | Single | Координата y конечной точки кривой (Единица: пиксель). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

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


            //добавить свободную форму
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });

            // Сохранить результат
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


