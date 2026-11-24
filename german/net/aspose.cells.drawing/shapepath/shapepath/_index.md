---
title: "ShapePath.ShapePath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePath‑Konstruktor. Initialisiert eine neue Instanz der ShapePath‑Klasse"
type: docs
url: /de/net/aspose.cells.drawing/shapepath/shapepath/
---
## ShapePath constructor

Initialisiert eine neue Instanz der [`ShapePath`](../)‑Klasse.

```csharp
public ShapePath()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstellen Sie einen neuen ShapePath mit der #ctor‑Methode
                ShapePath shapePath = new ShapePath();

                // Fügen Sie Pfadsegmente hinzu, um eine einfache Form zu erstellen
                shapePath.MoveTo(100, 100);
                shapePath.LineTo(200, 100);
                shapePath.LineTo(200, 200);
                shapePath.LineTo(100, 200);
                shapePath.Close();

                //Freiform hinzufügen
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath });

                Console.WriteLine("ShapePath created and added to worksheet successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("ShapePathMethodCtorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


