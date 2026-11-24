---
title: "PivotOptions.DropZoneData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotOptions-Eigenschaft. Gibt an, ob für jedes PivotTable-Feld auf der Datenachse der Quell-PivotTable ein Steuerelement im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist."
type: docs
url: /de/net/aspose.cells.charts/pivotoptions/dropzonedata/
---
## PivotOptions.DropZoneData property

Gibt an, ob ein Steuerelement für jedes PivotTable‑Feld auf der Datenachse der Quell‑PivotTable im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist.

```csharp
public bool DropZoneData { get; set; }
```

### Beispiele

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

            // Beispieldaten für PivotTable
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Books");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Books");
            worksheet.Cells["B4"].PutValue(1500);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Diagramm erstellen, das mit PivotTable verknüpft ist
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "SalesPivot";

            // Pivot-Optionen mit aktiviertem DropZoneData konfigurieren
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZonesVisible = true;

            // Ergebnis speichern
            workbook.Save("PivotOptionsDropZoneDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


