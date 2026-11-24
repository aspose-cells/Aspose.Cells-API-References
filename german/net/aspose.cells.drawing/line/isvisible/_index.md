---
title: "Line.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line-Eigenschaft. Gibt an, ob die Linie sichtbar ist"
type: docs
url: /de/net/aspose.cells.drawing/line/isvisible/
---
## Line.IsVisible property

Stellt dar, ob die Linie sichtbar ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
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
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Greifen Sie auf Hauptgitternetzlinien zu und setzen Sie die Sichtbarkeit
            chart.CategoryAxis.MajorGridLines.IsVisible = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Überprüfen Sie die Sichtbarkeit
            Console.WriteLine("Major Gridlines Visible: " + chart.CategoryAxis.MajorGridLines.IsVisible);
        }
    }
}
```

### Siehe auch

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


