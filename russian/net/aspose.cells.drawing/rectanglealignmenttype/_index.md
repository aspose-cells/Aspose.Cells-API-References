---
title: "Перечисление RectangleAlignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.RectangleAlignmentType. Представляет, как позиционировать два прямоугольника относительно друг друга"
type: docs
url: /ru/net/aspose.cells.drawing/rectanglealignmenttype/
---
## RectangleAlignmentType enumeration

Представляет способ позиционирования двух прямоугольников относительно друг друга.

```csharp
public enum RectangleAlignmentType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Bottom | `0` | Низ |
| BottomLeft | `1` | BottomLeft |
| BottomRight | `2` | BottomRight |
| Center | `3` | Center |
| Left | `4` | Left |
| Right | `5` | Right |
| Top | `6` | Top |
| TopLeft | `7` | TopLeft |
| TopRight | `8` | TopRight |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassRectangleAlignmentTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить форму прямоугольника для демонстрации выравнивания
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 200, 100, 100);

                // Продемонстрировать различные типы выравнивания
                Console.WriteLine("Available RectangleAlignmentType values:");
                Console.WriteLine("Bottom: " + RectangleAlignmentType.Bottom);
                Console.WriteLine("BottomLeft: " + RectangleAlignmentType.BottomLeft);
                Console.WriteLine("BottomRight: " + RectangleAlignmentType.BottomRight);
                Console.WriteLine("Center: " + RectangleAlignmentType.Center);
                Console.WriteLine("Left: " + RectangleAlignmentType.Left);
                Console.WriteLine("Right: " + RectangleAlignmentType.Right);
                Console.WriteLine("Top: " + RectangleAlignmentType.Top);
                Console.WriteLine("TopLeft: " + RectangleAlignmentType.TopLeft);
                Console.WriteLine("TopRight: " + RectangleAlignmentType.TopRight);

                // Установить выравнивание на основе одного из значений перечисления
                rectangle.TextHorizontalAlignment = TextAlignmentType.Center;
                rectangle.TextVerticalAlignment = TextAlignmentType.Center;

                // Сохраните книгу
                workbook.Save("RectangleAlignmentTypeDemo.xlsx");
                Console.WriteLine("RectangleAlignmentType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating RectangleAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


