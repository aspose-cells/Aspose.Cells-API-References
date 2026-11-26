---
title: "Shape.SoftEdges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает радиус размытия, применяемый к краям, в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/shape/softedges/
---
## Shape.SoftEdges property

Получает и задает радиус размытия, применяемый к краям, в единицах точек.

```csharp
public double SoftEdges { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySoftEdgesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Установить эффект мягких краев с радиусом 5 точек (0.5d = 5 точек)
            shape.SoftEdges = 0.5d;

            // Сохраните книгу
            workbook.Save("SoftEdgesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


