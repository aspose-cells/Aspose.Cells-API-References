---
title: "DataLabels.ShowLegendKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt das Anzeigeverhalten des Legenden-Schlüssels einer Diagrammdatenbeschriftung an. Wahr, wenn der Legenden-Schlüssel der Datenbeschriftung sichtbar ist"
type: docs
url: /de/net/aspose.cells.charts/datalabels/showlegendkey/
---
## DataLabels.ShowLegendKey property

Stellt das Anzeigeverhalten des Legenden-Schlüssels eines Datenlabels in einem bestimmten Diagramm dar. True, wenn der Legenden-Schlüssel des Datenlabels sichtbar ist.

```csharp
public bool ShowLegendKey { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowLegendKeyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen abrufen
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Setze ShowLegendKey auf wahr
            dataLabels.ShowLegendKey = true;
            Console.WriteLine("ShowLegendKey set to: " + dataLabels.ShowLegendKey);

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsShowLegendKeyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


