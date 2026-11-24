---
title: "ShapePath.Close"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePath-Methode. Schließt die aktuelle Figur und startet eine neue Figur. Wenn die aktuelle Figur eine Sequenz verbundener Linien und Kurven enthält, schließt die Methode die Schleife, indem sie eine Linie vom Endpunkt zum Startpunkt verbindet."
type: docs
url: /de/net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

Schließt die aktuelle Figur und startet eine neue Figur. Wenn die aktuelle Figur eine Sequenz verbundener Linien und Kurven enthält, schließt die Methode die Schleife, indem sie eine Linie vom Endpunkt zum Startpunkt verbindet.

```csharp
public void Close()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
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
                shapePath.MoveTo(60, 45);
                shapePath.ArcTo(25, 25, 0, 270);

                // Schließe den Pfad
                shapePath.Close();

                shapePath.MoveTo(60, 20);
                shapePath.LineTo(110, 70);
                shapePath.LineTo(125, 155.5f);
                shapePath.ArcTo(35.5f, 35.5f, 0, 270);

                // Schließe den Pfad
                shapePath.Close();

                //Freiform hinzufügen
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // Speichere die Arbeitsmappe
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


