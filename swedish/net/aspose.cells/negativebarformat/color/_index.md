---
title: "NegativeBarFormat.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NegativeBarFormat egenskap. Hämtar eller anger ett FormatColor-objekt som du kan använda för att ange fyllningsfärgen för negativa datastaplar"
type: docs
url: /sv/net/aspose.cells/negativebarformat/color/
---
## NegativeBarFormat.Color property

Hämtar eller anger ett FormatColor-objekt som du kan använda för att ange fyllningsfärgen för negativa datastaplar.

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
    public class NegativeBarFormatPropertyColorDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Skapa villkorlig formatering
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Ställ in egenskaper för datastaplar
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Ställ in format för negativa staplar
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Spara arbetsboken
            workbook.Save("NegativeBarFormatColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("NegativeBarFormatPropertyColorDemo executed successfully.");
        }
    }
}
```

### Se även

* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


