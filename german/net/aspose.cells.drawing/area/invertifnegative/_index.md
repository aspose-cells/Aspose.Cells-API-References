---
title: "Area.InvertIfNegative"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Area‑Eigenschaft. Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden Vordergrundfarbe und Hintergrundfarbe vertauscht"
type: docs
url: /de/net/aspose.cells.drawing/area/invertifnegative/
---
## Area.InvertIfNegative property

Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden die Vordergrundfarbe und die Hintergrundfarbe ausgetauscht.

```csharp
public bool InvertIfNegative { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyInvertIfNegativeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten mit negativem Wert hinzufügen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Spaltendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Datenreihen hinzufügen und Flächeneigenschaften konfigurieren
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Area.InvertIfNegative = true;
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.BackgroundColor = Color.Yellow;
            
            workbook.Save("AreaPropertyInvertIfNegativeDemo.xls");
        }
    }
}
```

### Siehe auch

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


