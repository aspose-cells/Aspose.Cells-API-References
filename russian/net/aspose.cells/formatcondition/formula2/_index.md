---
title: "FormatCondition.Formula2"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получает и задает значение или выражение, связанное с условным форматированием"
type: docs
url: /ru/net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

Получает и задает значение или выражение, связанное с условным форматированием.

```csharp
public string Formula2 { get; set; }
```

### Примечания

Пожалуйста, добавьте все области перед установкой формулы. При установке формулы для этого условия, если входное значение начинается с '=', оно будет восприниматься как формула. В противном случае оно будет восприниматься как простое значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\"=...\"".

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula2Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить условное форматирование
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[index];
            
            // Определите диапазон ячеек
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            
            // Добавьте условие форматирования с Formula2
            formatConditions.Add(area, 
                FormatConditionType.CellValue, 
                OperatorType.Between, 
                "=\"abc def\"", 
                "=\"a\"&\"b\"");

            // Получите условие форматирования
            FormatCondition formatCondition = formatConditions[0];

            // Выведите формулы
            Console.WriteLine("Formula1: " + formatCondition.Formula1);
            Console.WriteLine("Formula2: " + formatCondition.Formula2);

            // Сохраните книгу
            workbook.Save("FormatConditionFormula2Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


