---
title: "Перечисление GradientFillType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.GradientFillType. Представляет все типы градиентной заливки"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfilltype/
---
## GradientFillType enumeration

Представляет все типы заливки градиентом.

```csharp
public enum GradientFillType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Linear | `0` | Линейный |
| Radial | `1` | Радиальный |
| Rectangle | `2` | Прямоугольник |
| Path | `3` | Контур |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassGradientFillTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для демонстрации градиентной заливки
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 20);

            // Получить формат заливки
            FillFormat fillFormat = shape.Fill;

            // Установить тип градиентной заливки и свойства
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.Horizontal, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Вывести тип направления градиента
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Сохраните книгу
            workbook.Save("GradientFillTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


