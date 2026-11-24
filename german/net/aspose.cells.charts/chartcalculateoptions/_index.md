---
title: "Klasse ChartCalculateOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ChartCalculateOptions class. Stellt die Optionen für die Berechnung eines Diagramms dar"
type: docs
url: /de/net/aspose.cells.charts/chartcalculateoptions/
---
## ChartCalculateOptions class

Stellt die Optionen für die Berechnung eines Diagramms dar.

```csharp
public class ChartCalculateOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | Erstellt die Optionen für die Diagrammberechnung. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | Ob alle Datenpunkte bei der Diagrammberechnung aktualisiert werden sollen. Standard: False. Wenn Sie den Wert für jeden einzelnen Datenpunkt im Diagramm erhalten möchten, setzen Sie ihn auf true. Wird dieser Parameter auf True gesetzt, können beim Berechnen des Diagramms neue Datenpunkte erzeugt werden. Dies kann die Excel‑Datei vergrößern. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCalculateOptionsDemo
    {
        public static void ChartCalculateOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich für das Diagramm fest
            chart.SetChartDataRange("A1:B4", true);

            // Eine Instanz von ChartCalculateOptions erstellen
            ChartCalculateOptions options = new ChartCalculateOptions
            {
                UpdateAllPoints = true // Set the property to update all data points
            };

            // Das Diagramm mit den angegebenen Optionen berechnen
            chart.Calculate(options);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartCalculateOptionsExample.xlsx");
            workbook.Save("ChartCalculateOptionsExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


