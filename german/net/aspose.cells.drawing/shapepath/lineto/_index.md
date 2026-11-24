---
title: "ShapePath.LineTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePath-Methode. Fügt ein Liniensegment zur aktuellen Figur hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. Einheit Pixel"
type: docs
url: /de/net/aspose.cells.drawing/shapepath/lineto/
---
## ShapePath.LineTo method

Fügt ein Liniensegment zur aktuellen Figur hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. Einheit: Pixel.

```csharp
public void LineTo(float x, float y)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| x | Einzeln | Die x‑Koordinate des Endpunkts des Liniensegments (Einheit: Pixel). |
| y | Einzeln | Die y‑Koordinate des Endpunkts des Liniensegments (Einheit: Pixel). |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodLineToWithSingleSingleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Erstellen Sie einen neuen Formpfad
                ShapePath shapePath = new ShapePath();

                // Zum Ausgangspunkt bewegen
                shapePath.MoveTo(10, 10);
                
                // Rufen Sie die LineTo-Methode mit (Single, Single)-Parametern auf
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                //Freiform hinzufügen
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("LineTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("ShapePathMethodLineToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


