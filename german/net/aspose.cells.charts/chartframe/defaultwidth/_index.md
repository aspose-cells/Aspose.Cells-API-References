---
title: "ChartFrame.DefaultWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt die Breite der Standardposition in Einheiten von 1/4000 des Diagrammbereichs an"
type: docs
url: /de/net/aspose.cells.charts/chartframe/defaultwidth/
---
## ChartFrame.DefaultWidth property

Gibt die Breite der Standardposition in Einheiten von 1/4000 des Diagrammbereichs an.

```csharp
[Obsolete("Use ChartFrame.DefaultWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultWidth { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.DefaultWidthRatioToChart. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Greifen Sie auf den Diagrammtitel zu (der von ChartFrame erbt)
            Title title = chart.Title;
            
            // Zeigen Sie die Standardbreite des Diagrammrahmens an (in diesem Fall der Titel)
            Console.WriteLine("DefaultWidth of chart title: " + title.DefaultWidth);
            
            // Hinweis: DefaultWidth ist schreibgeschützt, daher können wir es nicht setzen
            // Wir können es nur lesen, um die Standardabmessungen zu verstehen
            
            // Demonstrieren Sie, wie diese Eigenschaft das Diagramm beeinflusst
            Console.WriteLine("IsDefaultPosBeSet: " + title.IsDefaultPosBeSet);
            Console.WriteLine("DefaultWidthRatioToChart: " + title.DefaultWidthRatioToChart);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartFrameDefaultWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


