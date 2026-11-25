---
title: "Top10.Rank"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Top10. Ottieni o imposta il valore di n in una regola di formattazione condizionale top/bottom n. Se IsPercent è true il valore deve essere compreso tra 0 e 100. Altrimenti deve essere compreso tra 0 e 1000. Il valore predefinito è 10"
type: docs
url: /it/net/aspose.cells/top10/rank/
---
## Top10.Rank property

Ottieni o imposta il valore di "n" in una regola di formattazione condizionale "top/bottom n". Se IsPercent è true, il valore deve essere compreso tra 0 e 100. Altrimenti deve essere compreso tra 0 e 1000. Il valore predefinito è 10.

```csharp
public int Rank { get; set; }
```

### Esempi

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

### Vedi anche

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


