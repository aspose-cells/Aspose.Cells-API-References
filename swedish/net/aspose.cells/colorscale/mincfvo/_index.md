---
title: "ColorScale.MinCfvo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ColorScale‑egenskap. Hämta eller ange detta ColorScales minsta värdeobjekt. Kan inte sätta null eller CFValueObject med typ FormatConditionValueType.Max till det"
type: docs
url: /sv/net/aspose.cells/colorscale/mincfvo/
---
## ColorScale.MinCfvo property

Hämta eller ange detta ColorScales minvärdesobjekt. Det går inte att sätta null eller CFValueObject med typen FormatConditionValueType.Max till det.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinCfvoDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Skapa en färgskala för villkorlig formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Lägg till färgskala
            int csIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            ColorScale cs = fcc[csIndex].ColorScale;

            // Ställ in MinCfvo‑egenskaper
            cs.MinCfvo.Type = FormatConditionValueType.Min;
            cs.MinCfvo.Value = "0";
            cs.MinColor = System.Drawing.Color.Red;

            // Ställ in MidCfvo‑egenskaper
            cs.MidCfvo.Type = FormatConditionValueType.Percentile;
            cs.MidCfvo.Value = "50";
            cs.MidColor = System.Drawing.Color.Yellow;

            // Ställ in MaxCfvo‑egenskaper
            cs.MaxCfvo.Type = FormatConditionValueType.Max;
            cs.MaxCfvo.Value = "0";
            cs.MaxColor = System.Drawing.Color.Green;

            // Spara arbetsboken
            workbook.Save("ColorScaleMinCfvoDemo.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


