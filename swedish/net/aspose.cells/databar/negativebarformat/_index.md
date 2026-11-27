---
title: "DataBar.NegativeBarFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar-egenskap. Hämtar NegativeBarFormat-objektet som är associerat med en villkorlig formateringsregel för en datastapel"
type: docs
url: /sv/net/aspose.cells/databar/negativebarformat/
---
## DataBar.NegativeBarFormat property

Hämtar NegativeBarFormat-objektet som är associerat med en data bar villkorsstyrd formateringsregel.

```csharp
public NegativeBarFormat NegativeBarFormat { get; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyNegativeBarFormatDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata med negativa värden
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Lägg till villkorlig formatering för datastaplar
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = sheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Ställ in egenskaper för datastaplar
            condition.DataBar.Color = Color.Orange;
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            condition.DataBar.ShowValue = false;

            // Ställ in kantegenskaper
            condition.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            condition.DataBar.BarBorder.Color = Color.Plum;

            // Ställ in fyllningstyp
            condition.DataBar.BarFillType = DataBarFillType.Gradient;

            // Ställ in axelns egenskaper
            condition.DataBar.AxisColor = Color.Red;
            condition.DataBar.AxisPosition = DataBarAxisPosition.Automatic;

            // Konfigurera negativ stapelformat
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Spara arbetsboken
            workbook.Save("DataBarNegativeFormatDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [NegativeBarFormat](../../negativebarformat/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


