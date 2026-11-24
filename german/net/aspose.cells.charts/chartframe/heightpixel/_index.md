---
title: "ChartFrame.HeightPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt die Höhe des Rahmens in Pixeln zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/chartframe/heightpixel/
---
## ChartFrame.HeightPixel property

Ruft die Höhe des Rahmens in Pixeln ab oder legt sie fest.

```csharp
public virtual int HeightPixel { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightPixelDemo
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
            
            // Zugriff auf den Diagrammtitel (der ein ChartFrame ist)
            ChartFrame chartTitle = chart.Title;
            
            // Aktuelle Höhe in Pixeln anzeigen
            Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
            
            // Legen Sie eine neue Höhe für den Titel fest
            chartTitle.HeightPixel = 40;
            Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
            
            // Zugriff auf die Legende (ein weiteres ChartFrame)
            ChartFrame legend = chart.Legend;
            
            // Legendenhöhe anzeigen und ändern
            Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
            legend.HeightPixel = 60;
            Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartFrameHeightPixelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


