---
title: "Row.IsBlank"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Указывает, содержит ли строка какие-либо данные"
type: docs
url: /ru/net/aspose.cells/row/isblank/
---
## Row.IsBlank property

Указывает, содержит ли строка какие-либо данные

```csharp
public bool IsBlank { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsBlankDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить первую строку (изначально пустую)
            Row row1 = worksheet.Cells.Rows[0];
            Console.WriteLine("Row 1 IsBlank: " + row1.IsBlank); // True
            
            // Добавить данные в первую строку
            worksheet.Cells["A1"].PutValue("Test");
            Console.WriteLine("Row 1 IsBlank after adding data: " + row1.IsBlank); // False
            
            // Создать еще одну пустую строку
            Row row2 = worksheet.Cells.Rows[1];
            Console.WriteLine("Row 2 IsBlank: " + row2.IsBlank); // True
            
            // Сравнить статус пустоты строки
            Console.WriteLine("Rows have same IsBlank status: " + (row1.IsBlank == row2.IsBlank)); // False
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


