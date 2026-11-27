---
title: "SolidFill.CellsColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SolidFill-egenskap. Hämtar och anger CellsColor-objektet"
type: docs
url: /sv/net/aspose.cells.drawing/solidfill/cellscolor/
---
## SolidFill.CellsColor property

Hämtar och anger `CellsColor`-objektet.

```csharp
public CellsColor CellsColor { get; set; }
```

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:A4", true);

            CellsColor cc = chart.NSeries[0].Area.FillFormat.SolidFill.CellsColor;
            cc.ThemeColor = new ThemeColor(ThemeColorType.Accent6, 0.6);
            chart.NSeries[0].Area.FillFormat.SolidFill.CellsColor = cc;

            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


