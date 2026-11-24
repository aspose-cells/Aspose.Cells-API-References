---
title: "ChartFrame.Height"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame‑Eigenschaft. Gibt die Höhe des Rahmens in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Gibt die Höhe des Rahmens in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Hinweise

Wie konvertiert man Einheiten von 1/4000 in Pixel? Höhe in Pixeln = Y * Chart.ChartObject.Height / 4000d;

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartFrame.HeightRatioToChart‑Eigenschaft. Höhe = HeightRatioToChart * 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Zugriff auf Datenbeschriftungen
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Setze Height‑Eigenschaft
            dataLabels.Height = 200; // Set height to 200 pixels
            
            // Zeige den Höhenwert an
            Console.WriteLine("DataLabels Height: " + dataLabels.Height);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartFramePropertyHeightDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


