---
title: "WorkbookSettings.QuotePrefixToStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorkbookSettings property. Указывает, применяется ли свойство QuotePrefix при вводе строкового значения, начинающегося с одинарной кавычки, в ячейку"
type: docs
url: /ru/net/aspose.cells/workbooksettings/quoteprefixtostyle/
---
## WorkbookSettings.QuotePrefixToStyle property

Указывает, применяется ли свойство [`QuotePrefix`](../../style/quoteprefix/) при вводе строкового значения (которое начинается с одинарной кавычки) в ячейку

```csharp
public bool QuotePrefixToStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyQuotePrefixToStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Включить QuotePrefixToStyle — строки, начинающиеся с ', получат стиль QuotePrefix
            workbook.Settings.QuotePrefixToStyle = true;
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.PutValue("'abc");
            Console.WriteLine("Cell A1 - QuotePrefix: " + cell1.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A1 - Value: " + cell1.StringValue);

            // Отключить QuotePrefixToStyle — строки сохраняют своё буквальное значение
            workbook.Settings.QuotePrefixToStyle = false;
            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.PutValue("'abc");
            Console.WriteLine("Cell A2 - QuotePrefix: " + cell2.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A2 - Value: " + cell2.StringValue);

            workbook.Save("QuotePrefixToStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


