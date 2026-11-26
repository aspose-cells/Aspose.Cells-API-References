---
title: "Shape.Glow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет объект GlowEffect, который задает эффект свечения для элемента диаграммы или фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/glow/
---
## Shape.Glow property

Представляет объект [`GlowEffect`](../../gloweffect/), который задает эффект свечения для элемента диаграммы или фигуры.

```csharp
public GlowEffect Glow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGlowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Получить доступ к эффекту свечения
            GlowEffect glow = shape.Glow;

            // Установить свойства свечения
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Purple;
            glow.Color = color;
            glow.Size = 10; // 10 point radius
            glow.Transparency = 0.5; // 50% transparency

            // Сохраните книгу
            workbook.Save("ShapeGlowDemo.xlsx");
        }
    }
}
```

### См. также

* class [GlowEffect](../../gloweffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


