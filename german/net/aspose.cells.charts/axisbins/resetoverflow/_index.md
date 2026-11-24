---
title: "AxisBins.ResetOverflow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AxisBins-Methode. Setzt den Überlauf zurück"
type: docs
url: /de/net/aspose.cells.charts/axisbins/resetoverflow/
---
## AxisBins.ResetOverflow method

Setze den Überlauf zurück

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetOverflow()
```

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Es handelt sich um eine interne Methode, die nicht extern aufgerufen werden muss, um Probleme zu vermeiden. Diese Eigenschaft wird 12 Monate nach Juli 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsMethodResetOverflowDemo
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

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hole die Werte-Achse
            Axis valueAxis = chart.ValueAxis;

            // Achsen-Bins erstellen
            AxisBins bins = valueAxis.Bins;

            // Überlaufwert festlegen
            bins.Overflow = 25;
            Console.WriteLine($"Overflow before reset: {bins.Overflow}");

            try
            {
                // Rufen Sie die Methode ResetOverflow auf
                bins.ResetOverflow();
                Console.WriteLine($"Overflow after reset: {bins.Overflow}");
                Console.WriteLine("ResetOverflow method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetOverflow method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("AxisBinsMethodResetOverflowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


