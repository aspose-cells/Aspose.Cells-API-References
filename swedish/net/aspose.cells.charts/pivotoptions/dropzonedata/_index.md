---
title: "PivotOptions.DropZoneData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotOptions-egenskap. Anger om en kontroll för varje PivotTable-fält på PivotTable‑dataaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true"
type: docs
url: /sv/net/aspose.cells.charts/pivotoptions/dropzonedata/
---
## PivotOptions.DropZoneData property

Anger om en kontroll för varje PivotTable‑fält på dataaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true.

```csharp
public bool DropZoneData { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldatat för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Books");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Books");
            worksheet.Cells["B4"].PutValue(1500);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa diagram länkat till pivottabell
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "SalesPivot";

            // Konfigurera pivotalternativ med DropZoneData aktiverat
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZonesVisible = true;

            // Spara resultatet
            workbook.Save("PivotOptionsDropZoneDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


