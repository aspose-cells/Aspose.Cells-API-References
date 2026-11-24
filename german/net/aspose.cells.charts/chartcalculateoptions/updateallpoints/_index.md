---
title: "ChartCalculateOptions.UpdateAllPoints"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartCalculateOptions‑Eigenschaft. Gibt an, ob beim Berechnen des Diagramms alle Datenpunkte aktualisiert werden sollen. Standardwert: False. Wenn Sie den Wert für jeden Datenpunkt im Diagramm erhalten möchten, setzen Sie sie speziell auf true. Wird dieser Parameter auf True gesetzt, können beim Berechnen des Diagramms neue Datenpunkte erzeugt werden. Dies kann die Excel‑Datei vergrößern."
type: docs
url: /de/net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

Ob alle Datenpunkte bei der Diagrammberechnung aktualisiert werden sollen. Standard: False. Wenn Sie den Wert für jeden einzelnen Datenpunkt im Diagramm erhalten möchten, setzen Sie ihn auf true. Wird dieser Parameter auf True gesetzt, können beim Berechnen des Diagramms neue Datenpunkte erzeugt werden. Dies kann die Excel‑Datei vergrößern.

```csharp
public bool UpdateAllPoints { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsPropertyUpdateAllPointsDemo
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
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(400);
            worksheet.Cells["C3"].PutValue(500);
            worksheet.Cells["C4"].PutValue(600);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Datenbeschriftungen aktivieren
            foreach (Aspose.Cells.Charts.Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
            }

            // Diagramm mit der Option UpdateAllPoints berechnen
            chart.Calculate(new Aspose.Cells.Charts.ChartCalculateOptions() { UpdateAllPoints = true });

            // Einige Datenbeschriftungswerte ausgeben, um das Ergebnis zu demonstrieren
            Console.WriteLine("Series1 Point1 Label: " + chart.NSeries[0].Points[0].DataLabels.Text);
            Console.WriteLine("Series2 Point2 Label: " + chart.NSeries[1].Points[1].DataLabels.Text);
        }
    }
}
```

### Siehe auch

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


