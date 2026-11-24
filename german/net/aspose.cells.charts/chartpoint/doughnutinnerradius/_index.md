---
title: "ChartPoint.DoughnutInnerRadius"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt den inneren Radius des Doughnut‑Segments in Pixeln zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für Doughnut‑Diagramme"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/doughnutinnerradius/
---
## ChartPoint.DoughnutInnerRadius property

Ermittelt den inneren Radius des Donut‑Segments in Pixeln nach Aufruf der Methode Chart.Calculate(). Gilt für Donut‑Diagramm.

```csharp
public int DoughnutInnerRadius { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDoughnutInnerRadiusDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // Füge ein Doughnut-Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechnen Sie das Diagramm, um die Diagrammpunkte zu erhalten
            chart.Calculate();

            // Hole den ersten ChartPoint aus der ersten Serie.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeigen Sie den aktuellen Wert von DoughnutInnerRadius an
            Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Hinweis: DoughnutInnerRadius ist schreibgeschützt, daher können wir ihn nicht direkt setzen
            // Um den inneren Radius zu ändern, müssen wir die HoleSize‑Eigenschaft des Diagramms anpassen
            chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available

            // Berechnen Sie das Diagramm neu, um DoughnutInnerRadius zu aktualisieren
            chart.Calculate();

            // Zeigen Sie den aktualisierten Wert von DoughnutInnerRadius an
            Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Speichere die Arbeitsmappe
            workbook.Save("DoughnutInnerRadiusDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


