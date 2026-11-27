---
title: "PivotOptions.DropZoneFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotOptions-egenskap. Anger om en kontroll för varje PivotTable-fält på PivotTable‑sidaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true"
type: docs
url: /sv/net/aspose.cells.charts/pivotoptions/dropzonefilter/
---
## PivotOptions.DropZoneFilter property

Anger om en kontroll för varje PivotTable‑fält på sidaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true.

```csharp
public bool DropZoneFilter { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
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

            // Skapa diagram länkat till pivot
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Konfigurera pivotalternativ med DropZoneFilter
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZonesVisible = true;

            workbook.Save("PivotOptionsDropZoneFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


