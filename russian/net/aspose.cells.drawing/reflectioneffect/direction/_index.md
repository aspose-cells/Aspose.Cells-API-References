---
title: "ReflectionEffect.Direction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReflectionEffect. Получает и задает направление градиентного альфа-наклона относительно самой фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/reflectioneffect/direction/
---
## ReflectionEffect.Direction property

Получает и задает направление альфа‑градиентной рампы относительно самой фигуры.

```csharp
public double Direction { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyDirectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру, чтобы применить эффект отражения
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Получите эффект отражения фигуры
            ReflectionEffect reflection = shape.Reflection;
            
            // Отобразите текущее значение Direction
            Console.WriteLine("Current Direction value: " + reflection.Direction);
            
            // Установите новое значение Direction (90 градусов)
            reflection.Direction = 90;
            Console.WriteLine("New Direction value: " + reflection.Direction);
            
            // Настройте другие свойства отражения для лучшей видимости
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            
            // Сохраните книгу, чтобы увидеть эффект отражения
            workbook.Save("ReflectionEffectDirectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


