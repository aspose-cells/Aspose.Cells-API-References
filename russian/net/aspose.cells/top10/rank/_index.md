---
title: "Top10.Rank"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Top10. Получить или установить значение n в условии форматирования top/bottom n. Если IsPercent равно true, значение должно быть от 0 до 100. В противном случае оно должно быть от 0 до 1000. Значение по умолчанию — 10"
type: docs
url: /ru/net/aspose.cells/top10/rank/
---
## Top10.Rank property

Получить или установить значение "n" в правиле условного форматирования "top/bottom n". Если IsPercent равно true, значение должно быть от 0 до 100. В противном случае оно должно быть от 0 до 1000. Значение по умолчанию — 10.

```csharp
public int Rank { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyRankDemo
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
            top10.Rank = 5;

            workbook.Save("Top10RankExample.xlsx");
        }
    }
}
```

### См. также

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


