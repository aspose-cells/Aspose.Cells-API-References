---
title: "Cell.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Возвращает номер строки, начиная с нуля, основанный на ячейке"
type: docs
url: /ru/net/aspose.cells/cell/row/
---
## Cell.Row property

Получает номер строки (нумерация с нуля) ячейки.

```csharp
public int Row { get; }
```

### Property Value

Номер строки ячейки

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте пример данных и формулу
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Найти ячейку, содержащую формулу
            Cell cell = worksheet.Cells.Find("=SUM(A1", null, new FindOptions()
            { 
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains 
            });
            
            // Продемонстрировать свойство Row
            Console.WriteLine("Formula found in row: " + cell.Row);
            Console.WriteLine("Formula found in column: " + cell.Column);
            
            // Проверьте, что строка правильная
            if (cell.Row == 2 && cell.Column == 0)
            {
                Console.WriteLine("Row property works correctly");
            }
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


