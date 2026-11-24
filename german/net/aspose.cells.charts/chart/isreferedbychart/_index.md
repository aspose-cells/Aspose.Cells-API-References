---
title: "Chart.IsReferedByChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Methode. Gibt zurück, ob die Zelle vom Diagramm referenziert wird"
type: docs
url: /de/net/aspose.cells.charts/chart/isreferedbychart/
---
## Chart.IsReferedByChart method

Gibt zurück, ob die Zelle vom Diagramm referenziert wird.

```csharp
[Obsolete("Use Chart.IsCellReferedByChart(int,int,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsReferedByChart(int rowIndex, int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Der Zeilenindex. |
| columnIndex | Int32 | Der Spalten‑Index |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode IsCellReferedByChart(int,int,int). Diese Methode wird 12 Monate nach April 2023 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsReferedByChartWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Prüfen, ob die Zelle B2 (Zeile 1, Spalte 1) vom Diagramm referenziert wird
                bool isReferred = chart.IsReferedByChart(1, 1);
                
                Console.WriteLine($"Is cell B2 referred by the chart? {isReferred}");
                
                // Prüfen Sie eine Zelle, die nicht im Diagrammdatenbereich liegt
                bool isNotReferred = chart.IsReferedByChart(10, 10);
                Console.WriteLine($"Is cell K11 referred by the chart? {isNotReferred}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsReferedByChart method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartMethodIsReferedByChartWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


