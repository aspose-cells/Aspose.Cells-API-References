---
title: "FormatCondition.SetFormulas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FormatCondition. Устанавливает значение или выражение, связанное с этим условием форматирования"
type: docs
url: /ru/net/aspose.cells/formatcondition/setformulas/
---
## FormatCondition.SetFormulas method

Задает значение или выражение, связанное с этим условием формата.

```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| formula1 | String | Значение или выражение, связанное с этим условием форматирования. Если входное значение начинается с '=', оно будет рассматриваться как формула. В противном случае оно будет рассматриваться как простое значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\"=...\"". |
| formula2 | String | Значение или выражение, связанное с этим условием форматирования. Формат ввода такой же, как у formula1 |
| isR1C1 | Boolean | Является ли формула формулой R1C1. |
| isLocal | Boolean | Является ли формула локализованной. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodSetFormulasWithStringStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int formatIndex = cfs.Add();
            FormatConditionCollection fcs = cfs[formatIndex];
            
            fcs.AddArea(CellArea.CreateCellArea("A1", "C10"));
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcs[conditionIndex];
            
            fc.Operator = OperatorType.Between;
            fc.SetFormulas("=1", "=2", false, false);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


