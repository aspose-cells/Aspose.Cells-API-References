---
title: "Shape.GetInputRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Получает диапазон, используемый для заполнения элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing/shape/getinputrange/
---
## Shape.GetInputRange method

Получает диапазон, используемый для заполнения элемента управления.

```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | Boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | Boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### Возвращаемое значение

Диапазон, используемый для заполнения элемента управления.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetInputRangeWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Input 1");
            worksheet.Cells["A2"].PutValue("Input 2");
            worksheet.Cells["A3"].PutValue("Input 3");

            // Добавить форму списка
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 0, 0);
            Shape shape = listBox;

            // Установить диапазон ввода для формы списка
            shape.SetInputRange("$A$1:$A$3", false, false);

            // Получить диапазон ввода
            string range = shape.GetInputRange(false, true);
            Console.WriteLine("Shape input range: " + range);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


