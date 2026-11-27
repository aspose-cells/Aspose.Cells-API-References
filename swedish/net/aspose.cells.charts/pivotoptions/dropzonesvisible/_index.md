---
title: "PivotOptions.DropZonesVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotOptions-egenskap. Anger om några pivotkontroller kan visas i pivotdiagrammet"
type: docs
url: /sv/net/aspose.cells.charts/pivotoptions/dropzonesvisible/
---
## PivotOptions.DropZonesVisible property

Anger om några pivåkontroller kan visas i pivådiagrammet.

```csharp
public bool DropZonesVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZonesVisibleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldatat för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa diagram länkat till pivottabell
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Konfigurera pivotalternativ med DropZonesVisible
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZonesVisible = true;

            workbook.Save("PivotOptionsDropZonesVisibleDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


