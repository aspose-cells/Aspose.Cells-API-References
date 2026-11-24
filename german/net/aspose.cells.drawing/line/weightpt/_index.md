---
title: "Line.WeightPt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line‑Eigenschaft. Gibt das Gewicht der Linie in Punkt‑Einheiten zurück oder legt es fest"
type: docs
url: /de/net/aspose.cells.drawing/line/weightpt/
---
## Line.WeightPt property

Liest oder setzt die Stärke der Linie in Punkten.

```csharp
public double WeightPt { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPtDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen konfigurieren
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.HasLeaderLines = true;

            // Leitlinien anpassen
            series.LeaderLines.IsAuto = false;
            series.LeaderLines.Style = Aspose.Cells.Drawing.LineType.Dot;
            series.LeaderLines.WeightPt = 0.25; // Demonstrate WeightPt property
            series.LeaderLines.Color = Color.LightCyan;

            // Speichere die Arbeitsmappe
            workbook.Save("LeaderLinesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


