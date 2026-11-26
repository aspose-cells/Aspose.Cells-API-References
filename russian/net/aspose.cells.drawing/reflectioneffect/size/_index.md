---
title: "ReflectionEffect.Size"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReflectionEffect. Получает и задает конечную позицию вдоль градиентного наклона альфа‑значения конечного альфа‑значения в процентах"
type: docs
url: /ru/net/aspose.cells.drawing/reflectioneffect/size/
---
## ReflectionEffect.Size property

Получает и задает конечную позицию (по альфа‑градиентной рампе) конечного альфа‑значения, в процентах.

```csharp
public double Size { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Установите свойства отражения, включая Size
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4;

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Проверьте сохранённые свойства отражения
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Reflection Size: " + loadedReflection.Size);
        }
    }
}
```

### См. также

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


