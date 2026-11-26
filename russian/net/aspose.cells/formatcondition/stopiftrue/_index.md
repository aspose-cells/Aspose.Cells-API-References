---
title: "FormatCondition.StopIfTrue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. True правила с более низким приоритетом не могут быть применены к этому правилу, когда оно оценивается как истинное. Применяется только для Excel 2007"
type: docs
url: /ru/net/aspose.cells/formatcondition/stopiftrue/
---
## FormatCondition.StopIfTrue property

True, правила с более низким приоритетом не могут применяться к этому правилу, когда оно оценивается как true. Применяется только к Excel 2007;

```csharp
public bool StopIfTrue { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStopIfTrueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Добавить условие и установить StopIfTrue
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            FormatCondition condition = fcs[conditionIndex];
            condition.StopIfTrue = true;
            
            // Добавить другое условие, которое обычно переопределяет первое
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "25", "");
            FormatCondition condition2 = fcs[conditionIndex2];
            condition2.StopIfTrue = false;

            // Сохраните книгу
            workbook.Save("StopIfTrueDemo.xlsx");
        }
    }
}
```

### См. также

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


