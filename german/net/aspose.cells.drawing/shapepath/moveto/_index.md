---
title: "ShapePath.MoveTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePath-Methode. Startet eine neue Figur vom angegebenen Punkt, ohne die aktuelle Figur zu schließen. Alle nachfolgenden Punkte, die dem Pfad hinzugefügt werden, gehören zu dieser neuen Figur. Einheit: Pixel"
type: docs
url: /de/net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

Startet eine neue Figur vom angegebenen Punkt, ohne die aktuelle Figur zu schließen. Alle nachfolgenden Punkte, die dem Pfad hinzugefügt werden, werden zu dieser neuen Figur hinzugefügt. Einheit: Pixel.

```csharp
public void MoveTo(float x, float y)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| x | Einzeln | Die x-Koordinate des Startpunkts der Figur (Einheit: Pixel). |
| y | Einzeln | Die y-Koordinate des Startpunkts der Figur (Einheit: Pixel). |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
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

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
           
            
            // Ergebnis speichern
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


