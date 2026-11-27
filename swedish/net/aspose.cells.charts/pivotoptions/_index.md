---
title: "Klass PivotOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.PivotOptions-klass. Representerar en komplex typ som specificerar pivåkontrollerna som visas i diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/pivotoptions/
---
## PivotOptions class

Representerar en komplex typ som specificerar pivåkontrollerna som visas i diagrammet

```csharp
public class PivotOptions
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DropZoneCategories](../../aspose.cells.charts/pivotoptions/dropzonecategories/) { get; set; } | Anger om en kontroll för varje PivotTable‑fält på radaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true. |
| [DropZoneData](../../aspose.cells.charts/pivotoptions/dropzonedata/) { get; set; } | Anger om en kontroll för varje PivotTable‑fält på dataaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true. |
| [DropZoneFilter](../../aspose.cells.charts/pivotoptions/dropzonefilter/) { get; set; } | Anger om en kontroll för varje PivotTable‑fält på sidaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true. |
| [DropZoneSeries](../../aspose.cells.charts/pivotoptions/dropzoneseries/) { get; set; } | Anger om en kontroll för varje PivotTable‑fält på kolumnaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true. |
| [DropZonesVisible](../../aspose.cells.charts/pivotoptions/dropzonesvisible/) { get; set; } | Anger om några pivåkontroller kan visas i pivådiagrammet. |
| [ShowExpandCollapseFieldButtons](../../aspose.cells.charts/pivotoptions/showexpandcollapsefieldbuttons/) { get; set; } | Hämtar eller anger ett värde som indikerar om expandera‑ eller kollapsa‑fältknappar ska visas |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotOptionsDemo
    {
        public static void PivotOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för pivåtabellen
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

            // Lägg till en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Åtkomst till PivotOptions i diagrammet
            PivotOptions pivotOptions = chart.PivotOptions;

            // Ställ in egenskaper för PivotOptions
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // Spara arbetsboken
            workbook.Save("PivotOptionsExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


