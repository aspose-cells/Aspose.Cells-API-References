---
title: "ConditionalFormattingValueCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ConditionalFormattingValueCollection. Добавляет объект ConditionalFormattingValue"
type: docs
url: /ru/net/aspose.cells/conditionalformattingvaluecollection/add/
---
## ConditionalFormattingValueCollection.Add method

Добавляет объект [`ConditionalFormattingValue`](../../conditionalformattingvalue/).

```csharp
public int Add(FormatConditionValueType type, string value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | FormatConditionValueType | Тип значения. |
| значение | String | Значение. |

### Возвращаемое значение

Возвращает индекс нового объекта в списке.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValueCollectionMethodAddWithFormatConditionValueTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];
            IconSet iconSet = cond.IconSet;
            iconSet.Type = IconSetType.Arrows3;

            ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;
            int cfvIndex = cfvos.Add(FormatConditionValueType.Number, "50");

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("ConditionalFormattingValueCollectionExample.xlsx");
        }
    }
}
```

### См. также

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


