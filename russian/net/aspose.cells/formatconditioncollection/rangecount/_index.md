---
title: "FormatConditionCollection.RangeCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatConditionCollection. Возвращает количество условно отформатированных диапазонов"
type: docs
url: /ru/net/aspose.cells/formatconditioncollection/rangecount/
---
## FormatConditionCollection.RangeCount property

Получает количество условно отформатированных диапазонов.

```csharp
public int RangeCount { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyRangeCountDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Добавлять диапазоны с помощью метода AddArea вместо AddRange
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "50");

            // Продемонстрировать свойство RangeCount
            Console.WriteLine($"Number of ranges in FormatConditionCollection: {fcc.RangeCount}");
            
            // Проверить RangeCount
            if (fcc.RangeCount < 1)
            {
                Console.WriteLine("Error: No ranges applied to conditional formatting");
            }
            else
            {
                Console.WriteLine("Conditional formatting ranges applied successfully");
            }
        }
    }
}
```

### См. также

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


