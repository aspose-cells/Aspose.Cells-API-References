---
title: "ReflectionEffect.RotWithShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReflectionEffect. Получает и задает, должно ли отражение вращаться вместе с формой"
type: docs
url: /ru/net/aspose.cells.drawing/reflectioneffect/rotwithshape/
---
## ReflectionEffect.RotWithShape property

Получает и задает, должно ли отражение вращаться вместе с фигурой.

```csharp
public bool RotWithShape { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyRotWithShapeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Создайте и примените эффект отражения
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.FullReflection4PtOffset;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Transparency = 0.3;

            // Отобразите текущее значение RotWithShape
            Console.WriteLine("Current RotWithShape value: " + reflection.RotWithShape);

            // Установите RotWithShape в true
            reflection.RotWithShape = true;
            Console.WriteLine("RotWithShape set to: " + reflection.RotWithShape);

            // Поверните форму, чтобы продемонстрировать эффект
            shape.RotationAngle = 45;

            // Сохраните книгу
            workbook.Save("ReflectionEffectRotWithShapeDemo.xlsx");
        }
    }
}
```

### См. также

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


