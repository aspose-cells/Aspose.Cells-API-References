---
title: "ChartFrame.WidthPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Liest oder schreibt die Breite des Rahmens in Einheiten von Pixel"
type: docs
url: /de/net/aspose.cells.charts/chartframe/widthpixel/
---
## ChartFrame.WidthPixel property

Ruft die Breite des Rahmens in Pixeln ab oder legt sie fest.

```csharp
public virtual int WidthPixel { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Greifen Sie auf den Diagrammtitel zu (der von ChartFrame erbt)
            chart.Title.Text = "Sample Chart";
            
            // Zeige den aktuellen WidthPixel-Wert des Diagrammtitels
            Console.WriteLine("Current Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Setze eine neue Breite für den Diagrammtitel in Pixel
            chart.Title.WidthPixel = 300;
            
            // Zeige den neuen WidthPixel-Wert
            Console.WriteLine("New Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartFrameWidthPixelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


