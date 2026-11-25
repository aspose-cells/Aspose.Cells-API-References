---
title: "Top10.IsBottom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Top10. Ottieni o imposta se una regola top/bottom n è una regola bottom n. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/top10/isbottom/
---
## Top10.IsBottom property

Ottieni o imposta se una regola "top/bottom n" è una regola "bottom n". Il valore predefinito è false.

```csharp
public bool IsBottom { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Aggiungi formattazione condizionale
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 0 });

            // Aggiungi condizione Top10
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Configura le proprietà Top10
            Top10 top10 = fc.Top10;
            top10.IsBottom = true; // Highlight bottom values
            top10.IsPercent = false;
            top10.Rank = 3; // Highlight bottom 3 values

            workbook.Save("Top10IsBottomExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


