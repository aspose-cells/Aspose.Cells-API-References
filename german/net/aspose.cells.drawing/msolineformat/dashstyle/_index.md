---
title: "MsoLineFormat.DashStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormat-Eigenschaft. Gibt den Strichstil für die angegebene Linie zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/msolineformat/dashstyle/
---
## MsoLineFormat.DashStyle property

Liest oder setzt den Strichstil für die angegebene Linie.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyDashStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Füge eine Form hinzu, um DashStyle zu demonstrieren
            Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Linieneigenschaften festlegen
            shape.LineFormat.Style = MsoLineStyle.Single;
            shape.LineFormat.Weight = 3;
            shape.LineFormat.ForeColor = Color.Blue;

            // Demonstriere verschiedene Strichstile
            shape.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            shape.Text = "Solid Line";

            // Füge eine weitere Form mit anderem Strichstil hinzu
            Shape shape2 = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 3, 0, 200, 100);
            shape2.LineFormat.Style = MsoLineStyle.Single;
            shape2.LineFormat.Weight = 3;
            shape2.LineFormat.ForeColor = Color.Red;
            shape2.LineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            shape2.Text = "DashDotDot Line";

            // Speichere die Arbeitsmappe
            workbook.Save("LineDashStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


