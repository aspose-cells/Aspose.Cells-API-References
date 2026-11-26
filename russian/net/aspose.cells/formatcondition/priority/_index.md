---
title: "FormatCondition.Priority"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Приоритет этого правила условного форматирования. Это значение используется для определения, какое форматирование следует оценить и отобразить. Меньшие числовые значения имеют более высокий приоритет, чем большие; 1 — самый высокий приоритет."
type: docs
url: /ru/net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

Приоритет этого правила условного форматирования. Это значение используется для определения, какой формат следует оценивать и применять. Меньшие числовые значения имеют более высокий приоритет, чем большие, где '1' — высший приоритет.

```csharp
public int Priority { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyPriorityDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Добавить условное форматирование
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            
            // Добавить условия
            int conditionIndex1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "2", "5");
            int conditionIndex2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "6", "9");

            // Установить приоритеты
            formatConditions[conditionIndex1].Priority = 2;
            formatConditions[conditionIndex2].Priority = 1;

            // Продемонстрировать использование свойства Priority
            Console.WriteLine("Condition 1 Priority: " + formatConditions[conditionIndex1].Priority);
            Console.WriteLine("Condition 2 Priority: " + formatConditions[conditionIndex2].Priority);

            // Сохраните книгу
            workbook.Save("ConditionalFormattingPriorityDemo.xlsx");
        }
    }
}
```

### См. также

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


