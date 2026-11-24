---
title: "ChartPoint.BorderWidthPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die Breite des Rahmens in Pixeln zurück, nachdem die Methode Chart.Calculate aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/borderwidthpx/
---
## ChartPoint.BorderWidthPx property

Ermittelt die Breite des Rahmens in Pixeln nach Aufruf der Methode Chart.Calculate().

```csharp
public int BorderWidthPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartPointPropertyBorderWidthPxDemo
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
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Fügen Sie ein Diagramm hinzu und setzen Sie dessen Datenbereich
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Diagramm berechnen, um sicherzustellen, dass Eigenschaften gefüllt sind
            chart.Calculate();

            // Den ersten Diagrammpunkt in der ersten Serie abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Anzeige der aktuellen Rahmenbreite
            Console.WriteLine("Current BorderWidthPx value: " + point.BorderWidthPx);

            // Hinweis: BorderWidthPx ist schreibgeschützt, daher können wir ihn nicht direkt setzen
            // Stattdessen können wir den Rahmen über die Border-Eigenschaft ändern
            if (point.Border != null)
            {
                // Ändere die Rahmenbreite, indem du das Gewicht mit dem WeightType-Enum festlegst
                point.Border.Weight = WeightType.MediumLine; // Medium weight border
            }

            // Neu berechnen, um den BorderWidthPx-Wert zu aktualisieren
            chart.Calculate();

            // Anzeige der neuen Rahmenbreite in Pixeln
            Console.WriteLine("New BorderWidthPx value after modification: " + point.BorderWidthPx);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyBorderWidthPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


