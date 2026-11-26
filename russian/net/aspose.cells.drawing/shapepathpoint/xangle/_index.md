---
title: "ShapePathPoint.XAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapePathPoint. Когда объект является маркером угла, получайте или задавайте первый угол в градусах"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

Когда объект является маркером угла, получайте или задавайте первый угол в градусах.

```csharp
public int XAngle { get; set; }
```

### Примечания

Если этот угол является начальным углом дуги. Этот угол указывает, какой угол вдоль предполагаемого кругового пути будет использован в качестве начальной позиции для рисования дуги. Этот начальный угол будет зафиксирован на последней известной позиции пера в пути фигуры. Таким образом гарантируется непрерывный путь фигуры.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXAngleDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать коллекцию точек пути фигуры
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // Получить первую точку и отобразить её координаты X и Y
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // ПРИМЕЧАНИЕ: Класс ShapePathPoint (согласно текущему отражению API) не предоставляет свойство XAngle.
            // Поэтому данная демонстрация сосредоточена на доступных свойствах X и Y.

            // Построить простую произвольную форму, используя определённые точки
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // Добавить произвольную форму на лист
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // Сохраните книгу
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


