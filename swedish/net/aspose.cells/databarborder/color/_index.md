---
title: "DataBarBorder.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBarBorder-egenskap. Hämtar eller anger kantens färg för datastaplar som specificeras av en villkorsstyrd formateringsregel"
type: docs
url: /sv/net/aspose.cells/databarborder/color/
---
## DataBarBorder.Color property

Hämtar eller anger kantens färg på datastaplarna som specificeras av en villkorsstyrd formateringsregel.

```csharp
public Color Color { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa en samling formatvillkor
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(new CellArea { StartRow = 2, StartColumn = 4, EndRow = 3, EndColumn = 6 });

            // Lägg till formatvillkor för datastapel
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Ställ in egenskaper för datastaplar
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Ange kantegenskaper (demonstrerar användning av Color)
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // Spara arbetsboken
            workbook.Save("DataBarBorderColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar border color demo completed.");
        }
    }
}
```

### Se även

* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


