---
title: "Top10.IsPercent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Top10-egenskap. Hämta eller ange om en top/bottom n-regel är en top/bottom n-procentregel. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/top10/ispercent/
---
## Top10.IsPercent property

Hämta eller ange om en \"top/bottom n\"‑regel är en \"top/bottom n percent\"‑regel. Standardvärdet är falskt.

```csharp
public bool IsPercent { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsPercentDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Lägg till en Top10-regel för villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);

            // Hämta Top10-formatvillkoret
            FormatCondition fc = fcc[0];
            
            // Ange Top10-egenskaper
            fc.Top10.IsPercent = true;  // Demonstrate IsPercent property
            fc.Top10.IsBottom = false;
            fc.Top10.Rank = 3;

            // Tillämpa formateringsstil
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Spara arbetsboken
            workbook.Save("Top10IsPercentDemo.xlsx");
        }
    }
}
```

### Se även

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


