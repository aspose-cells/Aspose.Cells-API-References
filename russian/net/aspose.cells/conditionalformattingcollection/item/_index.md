---
title: "ConditionalFormattingCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingCollection. Получает элемент FormatConditions по указанному индексу"
type: docs
url: /ru/net/aspose.cells/conditionalformattingcollection/item/
---
## ConditionalFormattingCollection indexer

Получает элемент FormatConditions по указанному индексу.

```csharp
public FormatConditionCollection this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Добавить условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            // Добавить условие форматирования
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "50");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Получить доступ и продемонстрировать использование свойства Item
            FormatConditionCollection firstFormatting = sheet.ConditionalFormattings[0];
            Console.WriteLine($"First formatting has {firstFormatting.Count} conditions");
            Console.WriteLine($"First condition operator: {firstFormatting[0].Operator}");
        }
    }
}
```

### См. также

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


