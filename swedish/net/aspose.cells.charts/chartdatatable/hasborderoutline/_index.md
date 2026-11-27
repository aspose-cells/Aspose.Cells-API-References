---
title: "ChartDataTable.HasBorderOutline"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartDataTable-egenskap. Sant om diagrammets datatabell har konturkanter"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/hasborderoutline/
---
## ChartDataTable.HasBorderOutline property

Sant om diagramdatatabellen har konturramar

```csharp
[Obsolete("Use ChartDataTable.HasOutlineBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderOutline { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället ChartDataTable.HasOutlineBorder-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderOutlineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Aktivera och konfigurera datatabell
            chart.ShowDataTable = true;
            ChartDataTable chartTable = chart.ChartDataTable;
            
            // Demonstrera HasBorderOutline-egenskapen
            chartTable.HasBorderOutline = true;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.Font.Color = Color.Blue;

            workbook.Save("ChartDataTableWithBorderOutline.xlsx");
        }
    }
}
```

### Se även

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


