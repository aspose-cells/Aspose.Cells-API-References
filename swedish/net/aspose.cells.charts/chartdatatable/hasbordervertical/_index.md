---
title: "ChartDataTable.HasBorderVertical"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartDataTable-egenskap. True om diagrammets datatabell har vertikala cellramar"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/hasbordervertical/
---
## ChartDataTable.HasBorderVertical property

Sant om diagramdatatabellen har vertikala cellramar

```csharp
[Obsolete("Use ChartDataTable.HasVerticalBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderVertical { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället ChartDataTable.HasVerticalBorder-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderVerticalDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.ShowDataTable = true;

            ChartDataTable chartTable = chart.ChartDataTable;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderHorizontal = true;

            workbook.Save("ChartDataTable_HasBorderVertical.xlsx");
        }
    }
}
```

### Se även

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


