---
title: "ReflectionEffect.Distance"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReflectionEffect. Получает и задает расстояние тени в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/reflectioneffect/distance/
---
## ReflectionEffect.Distance property

Получает и задает расстояние тени, в единицах точек.

```csharp
public double Distance { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму для тестирования отражения - фиксированные параметры, соответствующие сигнатуре метода
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Установить свойства отражения
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4; // Demonstrating Distance property

            // Сохранить и перезагрузить, чтобы проверить сохранность
            string outputPath = "ReflectionEffectDemo.xlsx";
            workbook.Save(outputPath);

            // Перезагрузить для проверки
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Original Distance: " + reflection.Distance);
            Console.WriteLine("Loaded Distance: " + loadedReflection.Distance);
        }
    }
}
```

### См. также

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


