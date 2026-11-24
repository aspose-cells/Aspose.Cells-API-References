---
title: "Klasse PivotOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.PivotOptions Klasse. Stellt einen komplexen Typ dar, der die Pivot-Steuerelemente angibt, die im Diagramm angezeigt werden."
type: docs
url: /de/net/aspose.cells.charts/pivotoptions/
---
## PivotOptions class

Stellt einen komplexen Typ dar, der die Pivot‑Steuerelemente spezifiziert, die im Diagramm erscheinen

```csharp
public class PivotOptions
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DropZoneCategories](../../aspose.cells.charts/pivotoptions/dropzonecategories/) { get; set; } | Gibt an, ob ein Steuerelement für jedes PivotTable‑Feld auf der Zeilenachse der Quell‑PivotTable im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist. |
| [DropZoneData](../../aspose.cells.charts/pivotoptions/dropzonedata/) { get; set; } | Gibt an, ob ein Steuerelement für jedes PivotTable‑Feld auf der Datenachse der Quell‑PivotTable im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist. |
| [DropZoneFilter](../../aspose.cells.charts/pivotoptions/dropzonefilter/) { get; set; } | Gibt an, ob ein Steuerelement für jedes PivotTable‑Feld auf der Seitenachse der Quell‑PivotTable im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist. |
| [DropZoneSeries](../../aspose.cells.charts/pivotoptions/dropzoneseries/) { get; set; } | Gibt an, ob ein Steuerelement für jedes PivotTable‑Feld auf der Spaltenachse der Quell‑PivotTable im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist. |
| [DropZonesVisible](../../aspose.cells.charts/pivotoptions/dropzonesvisible/) { get; set; } | Gibt an, ob beliebige Pivot‑Steuerelemente im Pivot‑Diagramm angezeigt werden können. |
| [ShowExpandCollapseFieldButtons](../../aspose.cells.charts/pivotoptions/showexpandcollapsefieldbuttons/) { get; set; } | Ermittelt oder legt einen Wert fest, der angibt, ob Expand‑ oder Collapse‑Feldschaltflächen angezeigt werden sollen. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Daten für die Pivot‑Tabelle hinzu
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

            // Fügen Sie eine Pivot-Tabelle hinzu
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Greifen Sie auf die PivotOptions des Diagramms zu
            PivotOptions pivotOptions = chart.PivotOptions;

            // Legen Sie Eigenschaften von PivotOptions fest
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // Speichere die Arbeitsmappe
            workbook.Save("PivotOptionsExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


