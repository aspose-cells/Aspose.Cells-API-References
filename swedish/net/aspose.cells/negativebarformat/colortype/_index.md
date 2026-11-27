---
title: "NegativeBarFormat.ColorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NegativeBarFormat egenskap. Hämtar eller anger om samma fyllningsfärg som för positiva datastaplar ska användas"
type: docs
url: /sv/net/aspose.cells/negativebarformat/colortype/
---
## NegativeBarFormat.ColorType property

Hämtar eller anger om samma fyllningsfärg som för positiva datastaplar ska användas.

```csharp
public DataBarNegativeColorType ColorType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-15);
            sheet.Cells["F4"].PutValue(25);
            sheet.Cells["G3"].PutValue(-5);
            sheet.Cells["G4"].PutValue(15);

            // Skapa intervall för villkorlig formatering
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Lägg till villkorlig formatering för datastaplar
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(area);
            
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Ställ in egenskaper för datastaplar
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            
            // Konfigurera negativ stapelformat
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Spara arbetsboken
            workbook.Save("NegativeBarFormatDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Demo completed. File saved with negative bar formatting.");
        }
    }
}
```

### Se även

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


