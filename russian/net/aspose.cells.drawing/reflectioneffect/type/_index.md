---
title: "ReflectionEffect.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReflectionEffect. Получает и задает предустановленный эффект отражения"
type: docs
url: /ru/net/aspose.cells.drawing/reflectioneffect/type/
---
## ReflectionEffect.Type property

Получает и задает предустановленный эффект отражения.

```csharp
public ReflectionEffectType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Получить эффект отражения
            ReflectionEffect reflection = shape.Reflection;
            
            // Продемонстрировать свойство Type
            Console.WriteLine("Initial reflection type: " + reflection.Type);
            
            // Изменить тип отражения
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            Console.WriteLine("Updated reflection type: " + reflection.Type);
            
            // Установите другие свойства отражения
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Сохраните книгу
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### См. также

* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


