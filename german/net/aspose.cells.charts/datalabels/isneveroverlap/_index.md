---
title: "DataLabels.IsNeverOverlap"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt an, ob Datenbeschriftungen niemals überlappen, wenn ein Kreisdiagramm in ein Bild umgewandelt wird. Hinweis: Diese Eigenschaft ist nur sinnvoll, wenn ein Kreisdiagramm in ein Bild umgewandelt wird."
type: docs
url: /de/net/aspose.cells.charts/datalabels/isneveroverlap/
---
## DataLabels.IsNeverOverlap property

Gibt an, ob DataLabels bei der Erstellung eines Kuchendiagramms als Bild niemals überlappen. Hinweis: Diese Eigenschaft ist nur sinnvoll, wenn ein Kuchendiagramm als Bild erstellt wird.

```csharp
public bool IsNeverOverlap { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsNeverOverlapDemo
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

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen aktivieren
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Datenbeschriftungen abrufen und die IsNeverOverlap-Eigenschaft festlegen
            DataLabels dataLabels = series.DataLabels;
            Console.WriteLine("Default IsNeverOverlap value: " + dataLabels.IsNeverOverlap);
            
            // Setze IsNeverOverlap auf wahr
            dataLabels.IsNeverOverlap = true;
            Console.WriteLine("After setting IsNeverOverlap: " + dataLabels.IsNeverOverlap);

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsIsNeverOverlapDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


