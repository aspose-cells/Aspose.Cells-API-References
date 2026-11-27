---
title: "Klassen ConditionalFormattingResult"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ConditionalFormattingResult-klass. Representerar resultatet av villkorsstyrd formatering som tillämpas på en cell"
type: docs
url: /sv/net/aspose.cells/conditionalformattingresult/
---
## ConditionalFormattingResult class

Representerar resultatet av villkorsstyrd formatering som tillämpas på en cell.

```csharp
public class ConditionalFormattingResult
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ColorScaleResult](../../aspose.cells/conditionalformattingresult/colorscaleresult/) { get; } | Hämtar visningsfärgen för färgskalan. |
| [ConditionalFormattingColorScale](../../aspose.cells/conditionalformattingresult/conditionalformattingcolorscale/) { get; } | Hämtar ColorScale-objektet. |
| [ConditionalFormattingDataBar](../../aspose.cells/conditionalformattingresult/conditionalformattingdatabar/) { get; } | Hämtar DataBar-objektet. |
| [ConditionalFormattingIcon](../../aspose.cells/conditionalformattingresult/conditionalformattingicon/) { get; } | Hämtar bilden av ikonsatsen. |
| [ConditionalStyle](../../aspose.cells/conditionalformattingresult/conditionalstyle/) { get; } | Hämtar den villkorsstyrda resultatstilen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingResultDemo
    {
        public static void ConditionalFormattingResultExample()
        {
            // Instansiera ett arbetsbok-objekt
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

            // Ställ in ColorScale-egenskaper
            fc.ColorScale.Is3ColorScale = true;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxColor = Color.Green;

            // Applicera några värden på cellerna
            for (int i = 0; i <= 10; i++)
            {
                for (int j = 0; j <= 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Hämta resultatet av villkorsstyrd formatering för en specifik cell
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult cfr = cell.GetConditionalFormattingResult();

            // Kom åt egenskaperna för ConditionalFormattingResult
            Style conditionalStyle = cfr.ConditionalStyle;
            ConditionalFormattingIcon icon = cfr.ConditionalFormattingIcon;
            DataBar dataBar = cfr.ConditionalFormattingDataBar;
            ColorScale colorScale = cfr.ConditionalFormattingColorScale;
            Color colorScaleResult = cfr.ColorScaleResult;

            // Visa några av egenskaperna
            Console.WriteLine("Conditional Style Background Color: " + (conditionalStyle != null ? conditionalStyle.BackgroundColor : Color.Empty));
            Console.WriteLine("Conditional Formatting Icon Type: " + (icon != null ? icon.Type.ToString() : "No Icon"));
            Console.WriteLine("Conditional Formatting DataBar Color: " + (dataBar != null ? dataBar.Color.ToString() : "No DataBar"));
            Console.WriteLine("Conditional Formatting ColorScale Min Color: " + (colorScale != null ? colorScale.MinColor.ToString() : "No ColorScale"));
            Console.WriteLine("Color Scale Result: " + colorScaleResult);

            // Spara arbetsboken
            workbook.Save("ConditionalFormattingResultExample.xlsx");
            workbook.Save("ConditionalFormattingResultExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


