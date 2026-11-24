---
title: "ChartFrame.IsAutomaticSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist"
type: docs
url: /de/net/aspose.cells.charts/chartframe/isautomaticsize/
---
## ChartFrame.IsAutomaticSize property

Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist.

```csharp
public virtual bool IsAutomaticSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsAutomaticSizeDemo
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

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Auf Legende zugreifen und die IsAutomaticSize‑Eigenschaft demonstrieren
            Aspose.Cells.Charts.Legend legend = chart.Legend;
            
            // Setze die automatische Größe auf false und zeige den Wert
            legend.IsAutomaticSize = false;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
            
            // Setze die automatische Größe auf true und zeige den Wert
            legend.IsAutomaticSize = true;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


