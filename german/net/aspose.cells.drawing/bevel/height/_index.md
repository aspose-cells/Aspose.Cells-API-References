---
title: "Bevel.Height"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Bevel Eigenschaft. Gibt die Höhe des Bevels zurück und legt sie fest, bzw. wie weit über die Form er angewendet wird. In Einheit von Punkten"
type: docs
url: /de/net/aspose.cells.drawing/bevel/height/
---
## Bevel.Height property

Liest und setzt die Höhe der Abschrägung bzw. wie weit über der Form sie angewendet wird. In Punkten.

```csharp
public double Height { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class BevelPropertyHeightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            // Ein 3D‑Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Zugriff auf das 3D-Format des Diagrammbereichs
            Format3D format3D = chart.PlotArea.ShapeProperties.Format3D;

            // Oberen Bevel mit Height-Eigenschaft konfigurieren
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.ArtDeco;
            topBevel.Width = 8;
            topBevel.Height = 4.5; // Demonstrating Height property usage

            // Speichere die Arbeitsmappe
            workbook.Save("BevelHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


