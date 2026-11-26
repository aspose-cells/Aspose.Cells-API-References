---
title: "Shape.CalculateTextSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Пересчитать область текста"
type: docs
url: /ru/net/aspose.cells.drawing/shape/calculatetextsize/
---
## Shape.CalculateTextSize method

Пересчитать область текста

```csharp
public int[] CalculateTextSize()
```

### Возвращаемое значение

Размер текста в массиве (ширина и высота).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCalculateTextSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пример текста в ячейку A1
            worksheet.Cells["A1"].PutValue("Sample Text for Size Calculation");

            // Создайте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Установите текст для формы
            shape.Text = "This is a test string to calculate text size";

            // Вычислите размер текста
            int[] size = shape.CalculateTextSize();

            // Выведите результаты
            Console.WriteLine($"Calculated text size - Width: {size[0]}, Height: {size[1]}");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


