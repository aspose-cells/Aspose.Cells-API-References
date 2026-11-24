---
title: "Chart.GapDepth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Diagramm-Eigenschaft. Gibt den Abstand zwischen den Datenserien in einem 3D-Diagramm als Prozentsatz der Markierungsbreite zurück oder legt ihn fest. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen."
type: docs
url: /de/net/aspose.cells.charts/chart/gapdepth/
---
## Chart.GapDepth property

Liefert oder setzt den Abstand zwischen den Datenreihen in einem 3‑D‑Diagramm als Prozentsatz der Markierungsbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen.

```csharp
public int GapDepth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyGapDepthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(110);
            worksheet.Cells["C4"].PutValue(130);

            // Ein 3D‑Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setzen Sie die GapDepth-Eigenschaft (steuert den Abstand zwischen Datenserien in 3D-Diagrammen)
            chart.GapDepth = 150; // Value between 0-500

            // Speichere die Arbeitsmappe
            workbook.Save("ChartGapDepthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


