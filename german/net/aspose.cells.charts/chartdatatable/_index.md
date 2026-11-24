---
title: "Klasse ChartDataTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ChartDataTable Klasse. Stellt eine Diagrammdatentabelle dar"
type: docs
url: /de/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

Stellt eine Diagrammdatentabelle dar.

```csharp
public class ChartDataTable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont/) { get; set; } | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. Der Standardwert ist True. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode/) { get; set; } | Liest und setzt den Anzeigemodus des Hintergrunds |
| [Border](../../aspose.cells.charts/chartdatatable/border/) { get; } | Gibt ein Border-Objekt zurück, das den Rand des Objekts darstellt |
| [Font](../../aspose.cells.charts/chartdatatable/font/) { get; } | Liest ein [`Font`](./font/) Objekt, das die Schriftarteinstellung der angegebenen Diagrammdatentabelle darstellt. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal/) { get; set; } | (**Obsolete.**) True, wenn die Diagrammdatentabelle horizontale Zellenränder hat |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline/) { get; set; } | (**Obsolete.**) True, wenn die Diagrammdatentabelle Umrandungsränder hat |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical/) { get; set; } | (**Obsolete.**) True, wenn die Diagrammdatentabelle vertikale Zellenränder hat |
| [HasHorizontalBorder](../../aspose.cells.charts/chartdatatable/hashorizontalborder/) { get; set; } | True, wenn die Diagrammdatentabelle horizontale Zellenränder hat |
| [HasOutlineBorder](../../aspose.cells.charts/chartdatatable/hasoutlineborder/) { get; set; } | True, wenn die Diagrammdatentabelle Umrandungsränder hat |
| [HasVerticalBorder](../../aspose.cells.charts/chartdatatable/hasverticalborder/) { get; set; } | True, wenn die Diagrammdatentabelle vertikale Zellenränder hat |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey/) { get; set; } | True, wenn der Legenden-Schlüssel der Datenbeschriftung sichtbar ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDataTableDemo
    {
        public static void ChartDataTableExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Ermitteln der Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];

            // Hinzufügen von Beispielwerten zu Zellen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];

            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von "A1"-Zelle bis "B3"
            chart.NSeries.Add("A1:B3", true);

            // Anzeigen der Datentabelle
            chart.ShowDataTable = true;

            // Abrufen der Diagrammdatentabelle
            ChartDataTable chartTable = chart.ChartDataTable;

            // Festlegen der Eigenschaften der Diagrammdatentabelle
            chartTable.Font.Color = Color.Red;
            chartTable.AutoScaleFont = true;
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderOutline = true;
            chartTable.ShowLegendKey = false;

            // Die Excel-Datei speichern
            workbook.Save("ChartDataTableExample.xlsx");
            workbook.Save("ChartDataTableExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


