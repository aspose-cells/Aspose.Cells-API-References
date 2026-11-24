---
title: "TickLabels.AutoScaleFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabels-Eigenschaft. Wahr, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße sich ändert. Der Standardwert ist Wahr"
type: docs
url: /de/net/aspose.cells.charts/ticklabels/autoscalefont/
---
## TickLabels.AutoScaleFont property

True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. Der Standardwert ist True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Beispieldaten
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(100000);
            cells["B3"].PutValue(150000);
            cells["B4"].PutValue(90000);

            // Diagramm erstellen
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdaten konfigurieren
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Achsenbeschriftungen mit AutoScaleFont konfigurieren
            chart.CategoryAxis.TickLabels.AutoScaleFont = true;
            chart.CategoryAxis.TickLabels.Font.Size = 12; // Initial size
            
            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelsAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


