---
title: "Class DataBar"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataBar class. Beskriv DataBar-regeln för villkorsstyrd formatering. Denna villkorsstyrda formateringsregel visar en graderad datastapel i cellintervallet"
type: docs
url: /sv/net/aspose.cells/databar/
---
## DataBar class

Beskriv regeln för villkorsstyrd formatering DataBar. Denna villkorsstyrda formateringsregel visar en graderad datastapel i cellområdet.

```csharp
public class DataBar
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor/) { get; set; } | Hämtar färgen på axeln för celler med villkorsstyrd formatering som datastaplar. |
| [AxisPosition](../../aspose.cells/databar/axisposition/) { get; set; } | Hämtar eller anger positionen för axeln på data bars som specificeras av en villkorsstyrd formateringsregel. |
| [BarBorder](../../aspose.cells/databar/barborder/) { get; } | Hämtar ett objekt som specificerar kanten på en data bar. |
| [BarFillType](../../aspose.cells/databar/barfilltype/) { get; set; } | Hämtar eller anger hur en data bar fylls med färg. |
| [Color](../../aspose.cells/databar/color/) { get; set; } | Hämta eller ange färgen för denna DataBar. |
| [Direction](../../aspose.cells/databar/direction/) { get; set; } | Hämtar eller anger riktningen som databar visas i. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo/) { get; } | Hämta eller ange detta DataBars maxvärdesobjekt. Det går inte att sätta null eller CFValueObject med typen FormatConditionValueType.Min till det. |
| [MaxLength](../../aspose.cells/databar/maxlength/) { get; set; } | Representerar den maximala längden på en data bar. |
| [MinCfvo](../../aspose.cells/databar/mincfvo/) { get; } | Hämta eller ange detta DataBars minvärdesobjekt. Det går inte att sätta null eller CFValueObject med typen FormatConditionValueType.Max till det. |
| [MinLength](../../aspose.cells/databar/minlength/) { get; set; } | Representerar den minsta längden på en data bar. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat/) { get; } | Hämtar NegativeBarFormat-objektet som är associerat med en data bar villkorsstyrd formateringsregel. |
| [ShowValue](../../aspose.cells/databar/showvalue/) { get; set; } | Hämta eller ange flaggan som indikerar om värdena i cellerna som denna data bar tillämpas på ska visas. Standardvärdet är true. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage/)(Cell, ImageOrPrintOptions) | Rendera data bar i cell till bildbytearray. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarDemo
    {
        public static void DataBarExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Ställer in området för den villkorliga formateringen
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Lägger till villkor
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Hämta DataBar
            DataBar dataBar = cond.DataBar;

            // Ange DataBar-egenskaper
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Sätt cellvärden
            Aspose.Cells.Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(10);
            Aspose.Cells.Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(120);
            Aspose.Cells.Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(260);

            // Sparar Excel-filen
            workbook.Save("DataBarExample.xlsx");
            workbook.Save("DataBarExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


