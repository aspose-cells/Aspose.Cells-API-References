---
title: "Klass NegativeBarFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.NegativeBarFormat-klass. Representerar färginställningarna för datastaplar för negativa värden som definieras av ett villkorligt formateringsregel för datastaplar"
type: docs
url: /sv/net/aspose.cells/negativebarformat/
---
## NegativeBarFormat class

Representerar färginställningarna för datastaplar för negativa värden som definieras av en villkorsstyrd formateringsregel för datastaplar.

```csharp
public class NegativeBarFormat
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BorderColor](../../aspose.cells/negativebarformat/bordercolor/) { get; set; } | Hämtar eller anger ett FormatColor-objekt som du kan använda för att ange kantfärgen för negativa datastaplar. |
| [BorderColorType](../../aspose.cells/negativebarformat/bordercolortype/) { get; set; } | Anger om samma kantfärg som för positiva datastaplar ska användas. |
| [Color](../../aspose.cells/negativebarformat/color/) { get; set; } | Hämtar eller anger ett FormatColor-objekt som du kan använda för att ange fyllningsfärgen för negativa datastaplar. |
| [ColorType](../../aspose.cells/negativebarformat/colortype/) { get; set; } | Hämtar eller anger om samma fyllningsfärg som för positiva datastaplar ska användas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class NegativeBarFormatDemo
    {
        public static void NegativeBarFormatExample()
        {
            // Instansiera ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Ställer in området för den villkorliga formateringen
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Lägger till ett villkor för DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Hämta DataBar och ange dess egenskaper
            DataBar dataBar = fc.DataBar;
            dataBar.Color = Color.Orange;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Konfigurera egenskaperna för NegativeBarFormat
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = Color.White;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = Color.Yellow;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;

            // Sätt in några värden i cellerna
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);

            // Spara arbetsboken
            workbook.Save("NegativeBarFormatExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


