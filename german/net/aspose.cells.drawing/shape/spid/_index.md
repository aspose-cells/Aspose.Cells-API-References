---
title: "Shape.Spid"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape Eigenschaft. Gibt einen optionalen Zeichenkettenbezeichner an, den eine Anwendung verwenden kann, um die jeweilige Form zu identifizieren."
type: docs
url: /de/net/aspose.cells.drawing/shape/spid/
---
## Shape.Spid property

Gibt einen optionalen Zeichenketten‑Bezeichner an, den eine Anwendung verwenden kann, um die jeweilige Form zu identifizieren.

```csharp
public string Spid { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySpidDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Rechteck-Shape zum Arbeitsblatt mit korrekten Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Die Spid-Eigenschaft der Form abrufen und anzeigen
            string spid = shape.Spid;
            Console.WriteLine("Shape SPID: " + spid);

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePropertySpidDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


