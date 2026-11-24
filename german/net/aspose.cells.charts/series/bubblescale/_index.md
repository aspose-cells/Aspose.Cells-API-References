---
title: "Series.BubbleScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe zurück oder legt ihn fest. Er kann ein ganzzahliger Wert von 0 bis 300 sein, entsprechend einem Prozentsatz der Standardgröße. Gilt nur für Blasendiagramme"
type: docs
url: /de/net/aspose.cells.charts/series/bubblescale/
---
## Series.BubbleScale property

Liest oder legt den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe fest. Er kann ein ganzzahliger Wert von 0 (null) bis 300 sein, was einem Prozentsatz der Standardgröße entspricht. Gilt nur für Blasendiagramme.

```csharp
public int BubbleScale { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleScaleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für Blasendiagramm hinzufügen
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["C1"].PutValue("Size");
            
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(5);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["C3"].PutValue(10);
            
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C4"].PutValue(15);

            // Ein Blasendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie zum Diagramm hinzufügen
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries[seriesIndex].XValues = "A2:A4";
            chart.NSeries[seriesIndex].BubbleSizes = "C2:C4";
            
            // Setzen Sie die Blasenskala, um die Eigenschaft zu demonstrieren
            chart.NSeries[seriesIndex].BubbleScale = 150; // Scale bubbles to 150% of default size
            
            // Das Aussehen des Diagramms anpassen
            chart.Title.Text = "Bubble Chart with Scaled Bubbles";
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.LightBlue, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            // Speichere die Arbeitsmappe
            workbook.Save("BubbleScaleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


