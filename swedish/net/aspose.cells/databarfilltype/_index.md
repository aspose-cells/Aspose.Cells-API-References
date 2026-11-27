---
title: "Enum DataBarFillType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataBarFillType enum. Anger hur en datastapel fylls med färg"
type: docs
url: /sv/net/aspose.cells/databarfilltype/
---
## DataBarFillType enumeration

Anger hur en datastapel fylls med färg.

```csharp
public enum DataBarFillType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Solid | `0` | Datastapeln är fylld med en solid färg. |
| Gradient | `1` | Datastapeln är fylld med en färggradient. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarFillTypeDemo
    {
        public static void DataBarFillTypeExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Lägger till ett nytt arbetsblad i arbetsboken
            Worksheet sheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Ställer in det villkorsstyrda formatintervallet.
            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Lägger till villkor
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Hämta Databar
            DataBar dataBar = cond.DataBar;

            // Ställ in Databar-egenskaper
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
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Sparar Excel-filen
            workbook.Save("DataBarFillTypeExample.xlsx");
            workbook.Save("DataBarFillTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


