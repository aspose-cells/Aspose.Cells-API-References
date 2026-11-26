---
title: "ReflectionEffect.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReflectionEffect. Получает и задает степень начальной прозрачности отражения в диапазоне от 0.0 (непрозрачный) до 1.0 (полностью прозрачный)"
type: docs
url: /ru/net/aspose.cells.drawing/reflectioneffect/transparency/
---
## ReflectionEffect.Transparency property

Получает и задает степень начальной прозрачности отражения в виде значения от 0,0 (непрозрачный) до 1,0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить прямоугольную форму на первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 150);
            
            // Получите эффект отражения и установите его свойства
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5; // Demonstrate transparency property
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Сохраните книгу
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Проверить сохранённые свойства
            Workbook loadedWorkbook = new Workbook("ReflectionEffectDemo.xlsx");
            Aspose.Cells.Drawing.ReflectionEffect loadedReflection = loadedWorkbook.Worksheets[0].Shapes[0].Reflection;
            
            Console.WriteLine("Reflection Type: " + loadedReflection.Type);
            Console.WriteLine("Transparency: " + loadedReflection.Transparency);
            Console.WriteLine("Size: " + loadedReflection.Size);
            Console.WriteLine("Blur: " + loadedReflection.Blur);
            Console.WriteLine("Distance: " + loadedReflection.Distance);
        }
    }
}
```

### См. также

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


