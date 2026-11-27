---
title: "NegativeBarFormat.BorderColorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NegativeBarFormat egenskap. Anger om samma kantfärg som för positiva datastaplar ska användas"
type: docs
url: /sv/net/aspose.cells/negativebarformat/bordercolortype/
---
## NegativeBarFormat.BorderColorType property

Anger om samma kantfärg som för positiva datastaplar ska användas.

```csharp
public DataBarNegativeColorType BorderColorType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyBorderColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Lägg till villkorlig formatering för datastaplar
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Ställ in datastapel
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Ställ in kant för datastapel
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // Ställ in format för negativ stapel
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            
            // Demonstrera BorderColorType egenskap
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Spara arbetsboken
            workbook.Save("NegativeBarFormatBorderColorTypeDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Demo completed. File saved.");
        }
    }
}
```

### Se även

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


