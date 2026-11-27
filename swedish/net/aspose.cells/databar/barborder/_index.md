---
title: "DataBar.BarBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar-egenskap. Hämtar ett objekt som specificerar kanten på en datastapel"
type: docs
url: /sv/net/aspose.cells/databar/barborder/
---
## DataBar.BarBorder property

Hämtar ett objekt som specificerar kanten på en data bar.

```csharp
public DataBarBorder BarBorder { get; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarBorderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Lägg till villkorlig formatering för datastaplar
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Lägg till villkor för datastapel
            int conditionIdx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIdx];

            // Ställ in egenskaper för datastaplar
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            fc.DataBar.Color = Color.Blue;
            fc.DataBar.ShowValue = true;

            // Ställ in stapelns kantegenskaper
            fc.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            fc.DataBar.BarBorder.Color = Color.Black;

            // Spara arbetsboken
            workbook.Save("DataBarBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataBarBorder](../../databarborder/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


