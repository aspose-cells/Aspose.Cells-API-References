---
title: "DataLabels.ShowBubbleSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt das Anzeigeverhalten des prozentualen Werts einer Diagrammdatenbeschriftung an. Wahr zeigt den Prozentwert an. Falsch blendet den Prozentwert aus"
type: docs
url: /de/net/aspose.cells.charts/datalabels/showbubblesize/
---
## DataLabels.ShowBubbleSize property

Stellt das Anzeigeverhalten des prozentualen Werts eines Datenlabels in einem bestimmten Diagramm dar. True zeigt den Prozentwert an. False blendet den Prozentwert aus.

```csharp
public bool ShowBubbleSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowBubbleSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Blasendiagramm hinzufügen
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(10);
            worksheet.Cells["C4"].PutValue(15);

            // Ein Blasendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Serie zum Diagramm hinzufügen
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Blasengrößen für die Serie festlegen
            Series series = chart.NSeries[seriesIndex];
            series.BubbleSizes = "C2:C4";

            // Auf die DataLabels der Serie zugreifen
            DataLabels dataLabels = series.DataLabels;

            // Demonstriere die ShowBubbleSize-Eigenschaft
            dataLabels.ShowBubbleSize = true; // Show bubble size in data labels
            dataLabels.ShowValue = true;      // Also show values for clarity

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsShowBubbleSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


