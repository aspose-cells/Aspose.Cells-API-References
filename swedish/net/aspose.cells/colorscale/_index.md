---
title: "Klass ColorScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ColorScale-klass. Beskriv ColorScale-regeln för villkorsstyrd formatering. Denna villkorsstyrda formateringsregel skapar en graderad färgskala på cellerna."
type: docs
url: /sv/net/aspose.cells/colorscale/
---
## ColorScale class

Beskriv regeln för villkorsstyrd formatering ColorScale. Denna villkorsstyrda formateringsregel skapar en graderad färgskala på cellerna.

```csharp
public class ColorScale
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Is3ColorScale](../../aspose.cells/colorscale/is3colorscale/) { get; set; } | Anger om villkorsstyrd formatering är en 3-färgs skala. |
| [MaxCfvo](../../aspose.cells/colorscale/maxcfvo/) { get; } | Hämta eller ange detta ColorScales maxvärdesobjekt. Det går inte att sätta null eller CFValueObject med typen FormatConditionValueType.Min till det. |
| [MaxColor](../../aspose.cells/colorscale/maxcolor/) { get; set; } | Hämta eller ange gradientfärgen för det maximala värdet i intervallet. |
| [MidCfvo](../../aspose.cells/colorscale/midcfvo/) { get; } | Hämta eller ange detta ColorScales mittvärdesobjekt. Det går inte att sätta CFValueObject med typen FormatConditionValueType.Max eller FormatConditionValueType.Min till det. |
| [MidColor](../../aspose.cells/colorscale/midcolor/) { get; set; } | Hämta eller ange gradientfärgen för mittvärdet i intervallet. |
| [MinCfvo](../../aspose.cells/colorscale/mincfvo/) { get; } | Hämta eller ange detta ColorScales minvärdesobjekt. Det går inte att sätta null eller CFValueObject med typen FormatConditionValueType.Max till det. |
| [MinColor](../../aspose.cells/colorscale/mincolor/) { get; set; } | Hämta eller ange gradientfärgen för det minsta värdet i intervallet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColorScaleDemo
    {
        public static void ColorScaleExample()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Lägg till en regel för villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 9 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Åtkomst till ColorScale-objektet
            ColorScale colorScale = fc.ColorScale;

            // Ställ in egenskaper för ColorScale
            colorScale.Is3ColorScale = true;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Ställ in min-, mitt- och maxvärdesobjekten
            ConditionalFormattingValue minCfvo = colorScale.MinCfvo;
            minCfvo.Type = FormatConditionValueType.Min;
            minCfvo.Value = null;

            ConditionalFormattingValue midCfvo = colorScale.MidCfvo;
            midCfvo.Type = FormatConditionValueType.Percentile;
            midCfvo.Value = 50;

            ConditionalFormattingValue maxCfvo = colorScale.MaxCfvo;
            maxCfvo.Type = FormatConditionValueType.Max;
            maxCfvo.Value = null;

            // Spara arbetsboken
            workbook.Save("ColorScaleExample.xlsx");
            workbook.Save("ColorScaleExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


