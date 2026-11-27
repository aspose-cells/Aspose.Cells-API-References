---
title: "DataBar.AxisColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar-egenskap. Hämtar färgen på axeln för celler med villkorsstyrd formatering som datastaplar"
type: docs
url: /sv/net/aspose.cells/databar/axiscolor/
---
## DataBar.AxisColor property

Hämtar färgen på axeln för celler med villkorsstyrd formatering som datastaplar.

```csharp
public Color AxisColor { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyAxisColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ange exempeldata
            sheet.Cells["E3"].PutValue(10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-15);
            sheet.Cells["G4"].PutValue(-25);

            // Lägg till villkorlig formatering för datastaplar
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Ställ in egenskaper för datastaplar
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;
            cond.DataBar.BarFillType = DataBarFillType.Solid;
            
            // Demonstrera AxisColor-egenskapen
            cond.DataBar.AxisColor = Color.Red;
            cond.DataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Ställ in negativ stapelformatering
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Spara arbetsboken
            workbook.Save("DataBarAxisColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


