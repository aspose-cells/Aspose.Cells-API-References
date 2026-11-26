---
title: "Row.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Получает ячейку"
type: docs
url: /ru/net/aspose.cells/row/item/
---
## Row indexer

Получает ячейку.

```csharp
public Cell this[int column] { get; }
```

| Параметр | Описание |
| --- | --- |
| column | Индекс столбца |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Получить доступ к первой строке
            Row row = sheet.Cells.Rows[0];
            
            // Установите HTML‑контент с разными цветовыми стилями
            row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
            row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
            
            // Продемонстрировать использование свойства Item и вывести цвета
            Console.WriteLine("Cell 0 Font Color: " + row[0].GetStyle().Font.Color.Name);
            Console.WriteLine("Cell 1 Font Color: " + row[1].GetStyle().Font.Color.Name);
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


