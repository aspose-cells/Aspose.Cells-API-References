---
title: "Chart.Calculate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Methode. Berechnet die benutzerdefinierten Positionen des Plot‑Bereichs und der Achsen, wenn deren Positionen automatisch zugewiesen werden"
type: docs
url: /de/net/aspose.cells.charts/chart/calculate/
---
## Calculate() {#calculate}

Berechnet die benutzerdefinierten Positionen des Plotbereichs und der Achsen, wenn deren Positionen automatisch zugewiesen werden.

```csharp
public void Calculate()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm vor dem Speichern berechnen
            chart.Calculate();

            // Arbeitsmappe mit Diagramm speichern
            workbook.Save("ChartCalculateDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Calculate(ChartCalculateOptions) {#calculate_1}

Berechnet die benutzerdefinierte Position von Plotbereich und Achsen, wenn deren Position automatisch zugewiesen wird, mit Chart Calculate Options.

```csharp
public void Calculate(ChartCalculateOptions calculateOptions)
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateWithChartCalculateOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen aktivieren
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Berechnungsoptionen erstellen und so einstellen, dass alle Punkte aktualisiert werden
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;

            // Diagramm mit Optionen berechnen
            chart.Calculate(calculateOptions);

            // Die Datenbeschriftungstexte ausgeben
            ChartPointCollection points = chart.NSeries[0].Points;
            Console.WriteLine("DataLabel Text for Point 0: " + points[0].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 1: " + points[1].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 2: " + points[2].DataLabels.Text);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartCalculateOptions](../../chartcalculateoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


