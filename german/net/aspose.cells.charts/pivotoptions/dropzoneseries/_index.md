---
title: "PivotOptions.DropZoneSeries"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotOptions-Eigenschaft. Gibt an, ob für jedes PivotTable-Feld auf der Spaltenachse der Quell-PivotTable ein Steuerelement im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist."
type: docs
url: /de/net/aspose.cells.charts/pivotoptions/dropzoneseries/
---
## PivotOptions.DropZoneSeries property

Gibt an, ob ein Steuerelement für jedes PivotTable‑Feld auf der Spaltenachse der Quell‑PivotTable im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist.

```csharp
public bool DropZoneSeries { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneSeriesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein Arbeitsblatt hinzufügen und das erste Blatt abrufen
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(7);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("A1:B4", true);
            
            // Pivot-Optionen aus dem Diagramm abrufen
            PivotOptions options = chart.PivotOptions;
            
            // DropZoneSeries-Eigenschaft demonstrieren
            Console.WriteLine("Original DropZoneSeries value: " + options.DropZoneSeries);
            options.DropZoneSeries = true;
            Console.WriteLine("Modified DropZoneSeries value: " + options.DropZoneSeries);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotOptionsPropertyDropZoneSeriesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


