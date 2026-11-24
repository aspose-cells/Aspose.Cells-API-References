---
title: "Enum DataLabelShapeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.DataLabelShapeType-Enum. Gibt die vordefinierte Formgeometrie an, die für ein Diagramm verwendet werden soll"
type: docs
url: /de/net/aspose.cells.drawing/datalabelshapetype/
---
## DataLabelShapeType enumeration

Gibt die voreingestellte Formgeometrie an, die für ein Diagramm verwendet werden soll.

```csharp
public enum DataLabelShapeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Rect | `0` | Stellt die Rechteckform dar. |
| RoundRect | `1` | Stellt die abgerundete Rechteckform dar. |
| Ellipse | `2` | Stellt die Ellipsenform dar. |
| RightArrowCallout | `3` | Stellt die Form des rechten Pfeil-Callouts dar. |
| DownArrowCallout | `4` | Stellt die Form des nach unten zeigenden Pfeil-Callouts dar. |
| LeftArrowCallout | `5` | Stellt die Form des linken Pfeil-Callouts dar. |
| UpArrowCallout | `6` | Stellt die Form des nach oben zeigenden Pfeil-Callouts dar. |
| WedgeRectCallout | `7` | Stellt die Form des Keil-Rechteck-Callouts dar. |
| WedgeRoundRectCallout | `8` | Stellt die Form des Keil-abgerundeten Rechteck-Callouts dar. |
| WedgeEllipseCallout | `9` | Stellt die Form des Keil-Ellipsen-Callouts dar. |
| LineCallout | `10` | Stellt die Form des Linien-Callouts dar. |
| BentLineCallout | `11` | Stellt die Form des gebogenen Linien-Callouts dar. |
| LineWithAccentBarCallout | `12` | Stellt die Form des Linien-Callouts mit Akzentleiste dar. |
| BentLineWithAccentBarCallout | `13` | Stellt die gebogene Linie mit Akzentbalken-Anmerkungsform dar. |
| Line | `14` | Dieser Typ wird nur für die spezielle Dateiverarbeitung verwendet |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class DataLabelShapeTypeDemo
    {
        public static void DataLabelShapeTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Greifen Sie auf die erste Serie im Diagramm zu
            Series series = chart.NSeries[0];

            // Datenbeschriftungen für die Serie aktivieren
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelShapeTypeExample.xlsx");
            workbook.Save("DataLabelShapeTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


