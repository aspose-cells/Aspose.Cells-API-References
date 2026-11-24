---
title: "Chart.IsChartDataChanged"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Methode. Erkennt, ob die Datenquelle des Diagramms geändert wurde"
type: docs
url: /de/net/aspose.cells.charts/chart/ischartdatachanged/
---
## Chart.IsChartDataChanged method

Erkennt, ob sich die Datenquelle eines Diagramms geändert hat.

```csharp
public bool IsChartDataChanged()
```

### Rückgabewert

Gibt true zurück, wenn das Diagramm geändert wurde, andernfalls false

### Hinweise

Die Methode erkennt die Änderungen in der Datenquelle des Diagramms, bevor das Diagramm in ein Bildformat gerendert wird. Beim ersten Aufruf von Chart.toImage werden die Diagrammdaten (z. B. XValuesParseData, ValuesParseData) aufgezeichnet. Bevor die Methode Chart.toImage erneut aufgerufen wird, rufen Sie die Methode IsChartDataChanged auf, um zu prüfen, ob das Diagramm neu gerendert werden muss.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsChartDataChangedDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Überprüfen, ob Diagrammdaten geändert wurden (sollte anfangs false sein)
                bool isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after creation: {isChanged}");

                // Diagrammdaten ändern
                worksheet.Cells["B2"].PutValue(15);

                // Erneut prüfen, ob Diagrammdaten geändert wurden
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after modification: {isChanged}");

                // Diagramm berechnen, um es zu aktualisieren
                chart.Calculate();

                // Nach der Berechnung prüfen
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after calculation: {isChanged}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsChartDataChanged method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("ChartMethodIsChartDataChangedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


