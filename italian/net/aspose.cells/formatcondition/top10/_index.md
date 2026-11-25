---
title: "FormatCondition.Top10"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottieni l'istanza Top10 della formattazione condizionale. La regola predefinita dell'istanza evidenzia le celle i cui valori rientrano nella fascia dei primi 10. Valida solo per il tipo Top10"
type: docs
url: /it/net/aspose.cells/formatcondition/top10/
---
## FormatCondition.Top10 property

Ottieni l'istanza "Top10" della formattazione condizionale. La regola dell'istanza predefinita evidenzia le celle i cui valori rientrano nella fascia top 10. Valida solo per type = Top10.

```csharp
public Top10 Top10 { get; }
```

### Esempi

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

### Vedi anche

* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


