---
title: "ReflectionEffect.Blur"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReflectionEffect. Получает и задает радиус размытия в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/reflectioneffect/blur/
---
## ReflectionEffect.Blur property

Получает и задает радиус размытия, в единицах точек.

```csharp
public double Blur { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить прямоугольную фигуру
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Получить доступ к эффекту отражения
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            
            // Установите тип отражения и свойства
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Blur = 0.5; // Demonstrate Blur property
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Distance = 0;
            
            // Сохраните книгу
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Отобразите значение размытия
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
        }
    }
}
```

### См. также

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


