---
title: "Shape.Fill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Возвращает объект FillFormat, содержащий свойства форматирования заливки для указанной фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/fill/
---
## Shape.Fill property

Возвращает объект [`FillFormat`](../fillformat/), содержащий свойства форматирования заливки для указанной фигуры.

```csharp
public FillFormat Fill { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFillDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Получите формат заполнения фигуры
            FillFormat fillFmt = shape.Fill;

            // Установить сплошное заполнение с цветом
            fillFmt.SolidFill.Color = System.Drawing.Color.Red;

            // Установить прозрачность
            fillFmt.Transparency = 0.5;

            // Сохраните книгу
            workbook.Save("ShapeFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [FillFormat](../../fillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


