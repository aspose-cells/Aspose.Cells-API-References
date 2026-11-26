---
title: "FormatCondition.Top10"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получить экземпляр условного форматирования Top10. Правило экземпляра по умолчанию выделяет ячейки, значения которых находятся в топ‑10. Действительно только для типа Top10"
type: docs
url: /ru/net/aspose.cells/formatcondition/top10/
---
## FormatCondition.Top10 property

Получить экземпляр "Top10" условного форматирования. Правило экземпляра по умолчанию выделяет ячейки, значения которых находятся в топ‑10. Действительно только для type = Top10.

```csharp
public Top10 Top10 { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTop10Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            Top10 top10 = fc.Top10;
            top10.IsPercent = true;
            top10.IsBottom = true;
            top10.Rank = 10;

            workbook.Save("FormatConditionPropertyTop10Demo.xlsx");
        }
    }
}
```

### См. также

* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


