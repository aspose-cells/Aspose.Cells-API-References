---
title: "Cell.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Копирует данные из исходной ячейки"
type: docs
url: /ru/net/aspose.cells/cell/copy/
---
## Cell.Copy method

Копирует данные из исходной ячейки.

```csharp
public void Copy(Cell cell)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cell | Cell | Исходный объект [`Cell`](../). |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCopyWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите значения и стили в исходной ячейке
            Cell sourceCell = cells["A1"];
            sourceCell.PutValue("Source Value");
            sourceCell.GetStyle().Font.IsBold = true;

            // Создайте целевую ячейку
            Cell destCell = cells["B1"];

            // Скопировать из исходного в целевой
            destCell.Copy(sourceCell);

            // Проверьте копию
            Console.WriteLine("Destination cell value: " + destCell.StringValue);
            Console.WriteLine("Destination cell bold status: " + destCell.GetStyle().Font.IsBold);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


