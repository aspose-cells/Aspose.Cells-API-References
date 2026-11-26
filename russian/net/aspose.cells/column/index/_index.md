---
title: "Column.Index"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Column. Получает индекс этого столбца"
type: docs
url: /ru/net/aspose.cells/column/index/
---
## Column.Index property

Получает индекс этого столбца.

```csharp
public int Index { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить некоторые данные в столбцы
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            
            // Получить коллекцию столбцов
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Продемонстрировать свойство Index
            Console.WriteLine("Column Indices:");
            for (int i = 0; i < columns.Count; i++)
            {
                Column column = columns[i];
                Console.WriteLine($"Column {column.Index}: {worksheet.Cells[0, column.Index].StringValue}");
            }
            
            // Доступ к столбцу по индексу
            Column columnB = columns[1]; // B column (index 1)
            Console.WriteLine($"\nAccessed by index 1: {worksheet.Cells[0, columnB.Index].StringValue}");
            
            // Изменить ширину столбца, используя индекс
            columns[2].Width = 30; // C column (index 2)
            Console.WriteLine($"\nColumn C width set to: {columns[2].Width}");
        }
    }
}
```

### См. также

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


