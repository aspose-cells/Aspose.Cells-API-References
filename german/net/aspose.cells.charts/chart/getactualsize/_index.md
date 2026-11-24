---
title: "Chart.GetActualSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Methode. Gibt die tatsächliche Größe des Diagramms in Pixeln zurück."
type: docs
url: /de/net/aspose.cells.charts/chart/getactualsize/
---
## Chart.GetActualSize method

Ermittelt die tatsächliche Größe des Diagramms in Pixel.

```csharp
public int[] GetActualSize()
```

### Rückgabewert

Tatsächliche Größe in einem Array (Breite und Höhe). [0] ist die Breite; [1] ist die Höhe.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodGetActualSizeDemo
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
                // Rufen Sie die Methode GetActualSize auf.
                int[] actualSize = chart.GetActualSize();
                
                // Ergebnis anzeigen
                Console.WriteLine($"Actual chart size - Width: {actualSize[0]}px, Height: {actualSize[1]}px");
                
                // Zeigen Sie den Effekt, indem Sie das Diagrammobjekt skalieren.
                chart.ChartObject.Width = actualSize[0];
                chart.ChartObject.Height = actualSize[1];
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetActualSize method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("ChartMethodGetActualSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


