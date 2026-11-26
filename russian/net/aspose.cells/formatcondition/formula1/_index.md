---
title: "FormatCondition.Formula1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получает и задает значение или выражение, связанное с условным форматированием"
type: docs
url: /ru/net/aspose.cells/formatcondition/formula1/
---
## FormatCondition.Formula1 property

Получает и задает значение или выражение, связанное с условным форматированием.

```csharp
public string Formula1 { get; set; }
```

### Примечания

Пожалуйста, добавьте все области перед установкой формулы. При установке формулы для этого условия, если входное значение начинается с '=', оно будет восприниматься как формула. В противном случае оно будет восприниматься как простое значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\"=...\"".

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula1Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["E1"].PutValue(50);
            
            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Установить диапазон и тип условия
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.LessOrEqual, "=$E$1<=100", null);
            
            // Получить доступ и отобразить свойство Formula1
            FormatCondition fc = fcc[0];
            Console.WriteLine("Formula1: " + fc.Formula1);
        }
    }
}
```

### См. также

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


