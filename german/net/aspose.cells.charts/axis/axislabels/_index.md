---
title: "Axis.AxisLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Achsen‑Eigenschaft. Gibt die Beschriftungen der Achse zurück, nachdem die Methode Chart.Calculate aufgerufen wurde"
type: docs
url: /de/net/aspose.cells.charts/axis/axislabels/
---
## Axis.AxisLabels property

Ermittelt die Beschriftungen der Achse nach Aufruf der Methode Chart.Calculate().

```csharp
[Obsolete("Use Axis.GetAxisTexts method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList AxisLabels { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Axis.GetAxisTexts. Diese Eigenschaft wird 12 Monate später, seit November 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyAxisLabelsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Füge dem Arbeitsblatt ein Diagramm hinzu
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Diagrammdatenbereich festlegen
                chart.NSeries.Add("B2:B4", true);
                chart.NSeries.CategoryData = "A2:A4";

                // Berechnen Sie das Diagramm, um Achsenbeschriftungen zu erzeugen
                chart.Calculate();

                // Greifen Sie auf die Kategorienachse zu und holen Sie die Achsenbeschriftungen
                Axis categoryAxis = chart.CategoryAxis;
                var axisLabels = categoryAxis.AxisLabels;

                // Achsenbeschriftungen anzeigen
                Console.WriteLine("Axis Labels:");
                if (axisLabels != null)
                {
                    foreach (var label in axisLabels)
                    {
                        Console.WriteLine(label);
                    }
                }
                else
                {
                    Console.WriteLine("No axis labels available.");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("AxisPropertyAxisLabelsDemo.xlsx");
                Console.WriteLine("AxisLabels demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


