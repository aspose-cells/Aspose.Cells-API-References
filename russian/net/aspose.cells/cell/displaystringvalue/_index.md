---
title: "Cell.DisplayStringValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Возвращает отформатированное строковое значение этой ячейки в соответствии со стилем отображения ячейки"
type: docs
url: /ru/net/aspose.cells/cell/displaystringvalue/
---
## Cell.DisplayStringValue property

Получает отформатированное строковое значение этой ячейки в соответствии со стилем отображения ячейки.

```csharp
public string DisplayStringValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDisplayStringValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Первый пример
            Style style = cell.GetStyle();
            style.Custom = "# ##/##\\\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: 3"
            
            // Второй пример
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3
            
            // Третий пример
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Четвёртый пример с десятичным значением
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1b c11d/e47f
            
            // Пятый пример с изменённым форматом
            style.Custom = "\"a\"#\"b\"\"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Шестой пример с десятичным значением
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1bc11d/e47f
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


