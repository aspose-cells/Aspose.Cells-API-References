---
title: "Класс ReflectionEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.ReflectionEffect класс. Этот класс определяет эффект отражения"
type: docs
url: /ru/net/aspose.cells.drawing/reflectioneffect/
---
## ReflectionEffect class

Этот класс задает эффект отражения.

```csharp
public class ReflectionEffect
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | Получает и задает радиус размытия, в единицах точек. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | Получает и задает направление альфа‑градиентной рампы относительно самой фигуры. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | Получает и задает расстояние тени, в единицах точек. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | Получает и задает направление смещения отражения. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | Получает и задает, должно ли отражение вращаться вместе с фигурой. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | Получает и задает конечную позицию (по альфа‑градиентной рампе) конечного альфа‑значения, в процентах. |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | Получает и задает степень начальной прозрачности отражения в виде значения от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | Получает и задает предустановленный эффект отражения. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Установить свойства эффекта отражения
            ReflectionEffect reflection = shape.Reflection;
            reflection.Size = 90;
            reflection.Blur = 30;
            reflection.Transparency = 0.5;
            reflection.Distance = 10;

            // Отобразить свойства отражения
            Console.WriteLine("Reflection Size: " + reflection.Size);
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
            Console.WriteLine("Reflection Transparency: " + reflection.Transparency);
            Console.WriteLine("Reflection Distance: " + reflection.Distance);

            // Сохраните книгу
            workbook.Save("ReflectionEffectDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


