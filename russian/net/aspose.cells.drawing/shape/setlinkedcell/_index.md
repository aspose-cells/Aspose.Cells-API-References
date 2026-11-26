---
title: "Shape.SetLinkedCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Устанавливает диапазон, связанный со значением элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing/shape/setlinkedcell/
---
## Shape.SetLinkedCell method

Задает диапазон, связанный со значением элемента управления.

```csharp
public void SetLinkedCell(string formula, bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Диапазон, связанный со значением элемента управления. |
| isR1C1 | Boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | Boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLinkedCellWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму ползунка
            Aspose.Cells.Drawing.Shape scrollBar = worksheet.Shapes.AddScrollBar(2, 0, 2, 0, 130, 30);

            // Связать значение ползунка с ячейкой A12
            scrollBar.SetLinkedCell("$A$12", false, true);

            // Сохраните книгу
            workbook.Save("SetLinkedCellDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


