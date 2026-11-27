---
title: "ColorScale.MinColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ColorScale-egenskap. Hämta eller ange gradientfärgen för det minsta värdet i intervallet"
type: docs
url: /sv/net/aspose.cells/colorscale/mincolor/
---
## ColorScale.MinColor property

Hämta eller ange gradientfärgen för det minsta värdet i intervallet.

```csharp
public Color MinColor { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Skapa ett CellArea‑objekt istället för att använda en sträng
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Konfigurera färgskala
            ColorScale colorScale = fc.ColorScale;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Ställ in värdetyper
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            colorScale.MidCfvo.Value = 50;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // Spara arbetsboken
            workbook.Save("ColorScaleMinColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


