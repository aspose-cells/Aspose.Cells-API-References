---
title: "Shape.GetActualBox"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Получить фактическое положение и размер фигуры после применения вращения, отражения и т.д."
type: docs
url: /ru/net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

Получить фактическое положение и размер фигуры (после применения вращения, отражения и т.д.)

```csharp
public float[] GetActualBox()
```

### Возвращаемое значение

Возвращает позицию и размер в порядке x, y, w, h

### Примечания

Примечание: Интерфейс не полностью функционален, особенно информация о местоположении некорректна. Рекомендуется не использовать этот интерфейс, пока функция не будет завершена.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetActualBoxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);

            // Получить фактические размеры коробки фигуры
            float[] box = rectangle.GetActualBox();

            // Вывести размеры коробки
            Console.WriteLine("Actual Box Dimensions:");
            Console.WriteLine($"Left: {box[0]}");
            Console.WriteLine($"Top: {box[1]}");
            Console.WriteLine($"Right: {box[2]}");
            Console.WriteLine($"Bottom: {box[3]}");

            // Сохраните книгу
            workbook.Save("ShapeGetActualBoxDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


