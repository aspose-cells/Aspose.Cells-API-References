---
title: "DataLabels.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt den Text der Datenbeschriftung zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/datalabels/text/
---
## DataLabels.Text property

Liest oder setzt den Text der Datenbeschriftung.

```csharp
public override string Text { get; set; }
```

### Hinweise

Funktioniert nur, wenn dies eine Datenbeschriftung eines Diagrammpunkts ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["A4"].PutValue("Product C");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen aktivieren
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Aspose.Cells.Charts.Series series = chart.NSeries[i];
                series.DataLabels.ShowValue = true;
                
                // Datenbeschriftungstext anpassen
                for (int j = 0; j < series.Points.Count; j++)
                {
                    series.Points[j].DataLabels.Text = $"+{series.Points[j].YValue}";
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsTextDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


