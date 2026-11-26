---
title: "Shape.InputRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает или задает диапазон листа, используемый для заполнения указанного комбинированного списка"
type: docs
url: /ru/net/aspose.cells.drawing/shape/inputrange/
---
## Shape.InputRange property

Получает или задает диапазон листа, используемый для заполнения указанного комбинированного списка.

```csharp
public string InputRange { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyInputRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["A2"].PutValue("Value 2");
            worksheet.Cells["A3"].PutValue("Value 3");
            worksheet.Cells["A4"].PutValue("Value 4");
            worksheet.Cells["A5"].PutValue("Value 5");

            // Добавить фигуру (прямоугольник)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Установить входной диапазон для фигуры
            shape.InputRange = "$A$1:$A$5";

            // Проверить и при необходимости изменить входной диапазон
            if (shape.InputRange.Equals("$A$1:$A$5"))
            {
                shape.InputRange = "$B$1:$B$5";
                Console.WriteLine("Input range changed to: " + shape.InputRange);
            }
            else
            {
                Console.WriteLine("Current input range: " + shape.InputRange);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


