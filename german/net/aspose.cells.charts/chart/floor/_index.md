---
title: "Chart.Floor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt ein Floor-Objekt zurück, das die Wände eines 3D-Diagramms darstellt"
type: docs
url: /de/net/aspose.cells.charts/chart/floor/
---
## Chart.Floor property

Gibt ein `Floor`-Objekt zurück, das die Wände eines 3‑D-Diagramms darstellt.

```csharp
public Floor Floor { get; }
```

### Hinweise

Diese Eigenschaft gilt nicht für 3‑D‑Kuchendiagramme.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyFloorDemo
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

            // Ein 3D‑Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Zugriff auf Bodeneigenschaften und deren Änderung
            Floor floor = chart.Floor;
            floor.FillFormat.SetTwoColorGradient(System.Drawing.Color.LightBlue, System.Drawing.Color.DarkBlue, GradientStyleType.Horizontal, 2);
            floor.Border.Color = System.Drawing.Color.Black;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartFloorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Floor](../../floor/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


