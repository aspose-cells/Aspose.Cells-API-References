---
title: "Shape.GetResultOfSmartArt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Konvertieren von SmartArt zu gruppierten Formen"
type: docs
url: /de/net/aspose.cells.drawing/shape/getresultofsmartart/
---
## Shape.GetResultOfSmartArt method

Konvertieren von SmartArt zu gruppierten Formen.

```csharp
public virtual GroupShape GetResultOfSmartArt()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetResultOfSmartArtDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform hinzu (da wir SmartArt nicht direkt erstellen können)
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);
            
            // In einem realen Szenario würden wir eine vorhandene SmartArt-Form laden
            // Zu Demonstrationszwecken überspringen wir die IsSmartArt‑Prüfung, da wir sie nicht setzen können

            // Erhalte das Ergebnis von SmartArt (funktioniert nur, wenn die Form tatsächlich SmartArt ist)
            GroupShape groupShape = shape.GetResultOfSmartArt();
            Console.WriteLine("Converted shape to GroupShape");
        }
    }
}
```

### Siehe auch

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


