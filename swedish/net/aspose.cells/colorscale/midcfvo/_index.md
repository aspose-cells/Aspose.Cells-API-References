---
title: "ColorScale.MidCfvo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ColorScale‑egenskap. Hämta eller ange detta ColorScales mittvärdeobjekt. Kan inte sätta CFValueObject med typ FormatConditionValueType.Max eller FormatConditionValueType.Min till det"
type: docs
url: /sv/net/aspose.cells/colorscale/midcfvo/
---
## ColorScale.MidCfvo property

Hämta eller ange detta ColorScales mittvärdesobjekt. Det går inte att sätta CFValueObject med typen FormatConditionValueType.Max eller FormatConditionValueType.Min till det.

```csharp
public ConditionalFormattingValue MidCfvo { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMidCfvoDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Lägg till en färgskala för villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            int conditionIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            
            // Ställ in mittpunktsvärdet för färgskalan
            ColorScale colorScale = fcc[conditionIndex].ColorScale;
            colorScale.MidCfvo.Type = FormatConditionValueType.Number;
            colorScale.MidCfvo.Value = 50;

            // Spara arbetsboken
            workbook.Save("ColorScalePropertyMidCfvoDemo.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


