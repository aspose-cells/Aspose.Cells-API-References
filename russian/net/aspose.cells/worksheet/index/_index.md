---
title: "Worksheet.Index"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает индекс листа в коллекции листов"
type: docs
url: /ru/net/aspose.cells/worksheet/index/
---
## Worksheet.Index property

Получает индекс листа в коллекции листов.

```csharp
public int Index { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить три листа
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Получить доступ к листам по индексу и продемонстрировать свойство Index
            Console.WriteLine("Worksheet Index Demonstration:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                Console.WriteLine($"Worksheet Name: {sheet.Name}, Index: {sheet.Index}");
            }

            // Добавить условное форматирование для демонстрации использования индекса
            Worksheet firstSheet = workbook.Worksheets[0];
            int formatIndex = firstSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = firstSheet.ConditionalFormattings[formatIndex];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Отобразить информацию об индексе условного форматирования
            Console.WriteLine("\nConditional Formatting Indexes:");
            Console.WriteLine($"Worksheet Index: {firstSheet.Index}");
            Console.WriteLine($"Formatting Collection Index: {formatIndex}");
            Console.WriteLine($"First Condition Index: 0");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


