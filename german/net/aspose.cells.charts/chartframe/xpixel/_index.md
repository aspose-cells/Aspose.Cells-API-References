---
title: "ChartFrame.XPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt die x‑Koordinate der oberen linken Ecke in Pixel‑Einheiten zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/chartframe/xpixel/
---
## ChartFrame.XPixel property

Liest oder legt fest die x‑Koordinate der oberen linken Ecke in Einheiten von Pixel.

```csharp
public virtual int XPixel { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Greifen Sie auf den Diagrammtitel zu (der von ChartFrame erbt)
            chart.Title.Text = "Sample Chart";
            
            // Aktuelle XPixel‑Position des Titels anzeigen
            Console.WriteLine("Current Title XPixel position: " + chart.Title.XPixel);
            
            // Verschieben Sie den Titel horizontal, indem Sie XPixel ändern
            chart.Title.XPixel = 200;
            
            // Neue XPixel‑Position anzeigen
            Console.WriteLine("New Title XPixel position: " + chart.Title.XPixel);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartFrameXPixelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


