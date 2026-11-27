---
title: "Klass ConditionalFormattingValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ConditionalFormattingValue-klass. Beskriver värdena för interpolationspunkterna i en gradientskala dataBar eller iconSet"
type: docs
url: /sv/net/aspose.cells/conditionalformattingvalue/
---
## ConditionalFormattingValue class

Beskriver värdena för interpolationspunkterna i en gradientskala, dataBar eller iconSet.

```csharp
public class ConditionalFormattingValue
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IsGTE](../../aspose.cells/conditionalformattingvalue/isgte/) { get; set; } | Hämta eller ange flaggan Greater Than Or Equal. Använd endast för ikonuppsättningar, bestämmer om detta tröskelvärde använder operatorn större än eller lika med. 'false' indikerar att 'greater than' används istället för 'greater than or equal to'. Standardvärdet är true. |
| [Type](../../aspose.cells/conditionalformattingvalue/type/) { get; set; } | Hämta eller ange typen för detta villkorsformateringsvärdeobjekt. Att ange typen till FormatConditionValueType.Min eller FormatConditionValueType.Max kommer automatiskt att sätta "Value" till null. |
| [Value](../../aspose.cells/conditionalformattingvalue/value/) { get; set; } | Hämta eller ange värdet för detta villkorsformateringsvärdeobjekt. Det bör användas tillsammans med Type. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingValueDemo
    {
        public static void ConditionalFormattingValueExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Ställer in området för den villkorliga formateringen
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Lägger till villkor
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Ställer in egenskaper för ColorScale
            fc.ColorScale.Is3ColorScale = true;

            // Ställer in minvärde
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // Ställer in mittvärde
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // Ställer in maxvärde
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // Spara arbetsboken
            workbook.Save("ConditionalFormattingValueExample.xlsx");
            workbook.Save("ConditionalFormattingValueExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


