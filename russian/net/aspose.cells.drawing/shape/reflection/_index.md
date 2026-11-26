---
title: "Shape.Reflection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет объект ReflectionEffect, который задает эффект отражения для элемента диаграммы или формы"
type: docs
url: /ru/net/aspose.cells.drawing/shape/reflection/
---
## Shape.Reflection property

Представляет объект [`ReflectionEffect`](../../reflectioneffect/), который задает эффект отражения для элемента диаграммы или формы.

```csharp
public ReflectionEffect Reflection { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyReflectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Установить свойства отражения
            ReflectionEffect reflection = shape.Reflection;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Direction = 90;
            reflection.FadeDirection = 90;
            reflection.Size = 50;
            reflection.Transparency = 0.5;
            reflection.Type = ReflectionEffectType.None;

            // Сохраните книгу
            workbook.Save("ShapeReflectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ReflectionEffect](../../reflectioneffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


