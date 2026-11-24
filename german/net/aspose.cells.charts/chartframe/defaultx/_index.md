---
title: "ChartFrame.DefaultX"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Stellt x der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar"
type: docs
url: /de/net/aspose.cells.charts/chartframe/defaultx/
---
## ChartFrame.DefaultX property

Stellt x der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar.

```csharp
[Obsolete("Use ChartFrame.DefaultXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultX { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.DefaultXRatioToChart. DefaultX = (int)(DefaultXRatioToChart * 4000); Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Greifen Sie auf den Diagrammtitel zu, der von ChartFrame erbt
            chart.Title.Text = "Sample Chart";
            
            // Zeigen Sie die standardmäßige X-Position des Diagrammtitels an
            Console.WriteLine("Default X position (1/4000 of chart area): " + chart.Title.DefaultX);
            Console.WriteLine("Default X position (ratio of chart area): " + chart.Title.DefaultXRatioToChart);
            
            // Demonstrieren Sie, wie die Standardposition das Diagramm beeinflusst
            Console.WriteLine("Is default position set? " + chart.Title.IsDefaultPosBeSet);
            
            // Ändern Sie die Position des Titels mithilfe von Verhältnis‑Eigenschaften (da DefaultX schreibgeschützt ist)
            chart.Title.XRatioToChart = 0.2;
            chart.Title.YRatioToChart = 0.05;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartFrameDefaultXDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


