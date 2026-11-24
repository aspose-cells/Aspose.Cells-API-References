---
title: "Area.FillFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Area-Eigenschaft. Stellt ein FillFormat-Objekt dar, das Füllformatierungs-Eigenschaften für das angegebene Diagramm oder die Form enthält"
type: docs
url: /de/net/aspose.cells.drawing/area/fillformat/
---
## Area.FillFormat property

Stellt ein `FillFormat`-Objekt dar, das Füllformatierungs-Eigenschaften für das angegebene Diagramm oder die Form enthält.

```csharp
public FillFormat FillFormat { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyFillFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Den dritten Punkt der ersten Reihe abrufen
            ChartPoint point = chart.NSeries[0].Points[2];
            
            // Füllformat-Eigenschaften festlegen
            point.Area.FillFormat.Pattern = FillPattern.DashedHorizontal;
            point.Area.FillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.Horizontal, 2);

            // Speichere die Arbeitsmappe
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


