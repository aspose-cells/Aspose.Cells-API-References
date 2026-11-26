---
title: "Shape.SetInputRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Устанавливает диапазон, используемый для заполнения элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing/shape/setinputrange/
---
## Shape.SetInputRange method

Задает диапазон, используемый для заполнения элемента управления.

```csharp
public void SetInputRange(string formula, bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Диапазон, используемый для заполнения элемента управления. |
| isR1C1 | Boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | Boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetInputRangeWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать объект рабочей книги
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки A1:A10
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Добавить форму списка
            Aspose.Cells.Drawing.Shape listBox = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);

            // Установить диапазон ввода для списка (используя параметры String, Boolean, Boolean)
            listBox.SetInputRange("$A$1:$A$6", false, false);

            // Установить связанную ячейку для списка
            listBox.SetLinkedCell("$A$12", false, true);

            // Сохраните книгу
            workbook.Save("SetInputRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


