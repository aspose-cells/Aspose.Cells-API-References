---
title: "Cell.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Возвращает номер столбца, начиная с нуля, для ячейки"
type: docs
url: /ru/net/aspose.cells/cell/column/
---
## Cell.Column property

Получает номер столбца (нумерация с нуля) ячейки.

```csharp
public int Column { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к ячейкам и продемонстрируйте свойство Column
            Cell cell1 = worksheet.Cells["A1"];
            Cell cell2 = worksheet.Cells["B2"];
            Cell cell3 = worksheet.Cells["C3"];

            // Установите значения и стили
            cell1.PutValue("Cell A1");
            cell2.PutValue("Cell B2");
            cell3.PutValue("Cell C3");

            // Продемонстрировать использование свойства Column
            Console.WriteLine("Cell A1 is in column: " + cell1.Column);
            Console.WriteLine("Cell B2 is in column: " + cell2.Column);
            Console.WriteLine("Cell C3 is in column: " + cell3.Column);

            // Измените ширину столбца с помощью свойства Column
            worksheet.Cells.Columns[cell1.Column].Width = 20;
            worksheet.Cells.Columns[cell2.Column].Width = 25;
            worksheet.Cells.Columns[cell3.Column].Width = 30;

            // Сохраните книгу
            workbook.Save("ColumnPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


