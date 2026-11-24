---
title: "Axis.DisplayUnitLabel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Stellt ein Einheitsetikett auf einer Achse im angegebenen Diagramm dar. Einheitsetiketten sind nützlich, um große Werte zu visualisieren, zum Beispiel in Millionen oder Milliarden."
type: docs
url: /de/net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

Stellt eine Einheitbeschriftung auf einer Achse im angegebenen Diagramm dar. Einheitbeschriftungen sind nützlich für die Darstellung großer Werte – zum Beispiel in Millionen oder Milliarden.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("A1:A4", true);
            
            // Anzeigeeinheit und Etikett konfigurieren
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Geben Sie den Text des Anzeigeeinheitsetiketts aus
            Console.WriteLine("Display Unit Label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Speichere die Arbeitsmappe
            workbook.Save("AxisPropertyDisplayUnitLabelDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


