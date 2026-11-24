---
title: "DrawObject.TotalPages"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DrawObject-Eigenschaft. Gibt die Gesamtseitenzahl der aktuellen Renderung an"
type: docs
url: /de/net/aspose.cells.rendering/drawobject/totalpages/
---
## DrawObject.TotalPages property

Gibt die Gesamtseitenzahl im aktuellen Rendering an.

```csharp
public int TotalPages { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyTotalPagesDemo
    {
        // Benutzerdefinierter Handler zum Erfassen von DrawObject-Ereignissen und zum Auslesen der TotalPages-Eigenschaft
        private class TotalPagesHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Den Wert der TotalPages-Eigenschaft anzeigen
                Console.WriteLine($"Total Pages in Rendering: {drawObject.TotalPages}");
                Console.WriteLine($"Current Page: {drawObject.CurrentPage + 1}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Fügen Sie Beispieldaten hinzu, um das Rendering sinnvoll zu machen
                sheet.Cells["A1"].PutValue("Sample Data");
                sheet.Cells["A2"].PutValue("More Data");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Eine Form hinzufügen, um sicherzustellen, dass mehrere DrawObjects erzeugt werden
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Richten Sie die Rendering‑Optionen mit unserem benutzerdefinierten Handler ein
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = false, // Allow multiple pages to demonstrate TotalPages
                    DrawObjectEventHandler = new TotalPagesHandler()
                };

                // Rendern Sie das Arbeitsblatt – dies löst die DrawObject‑Ereignisse aus
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "TotalPagesDemo.png");

                // Speichere die Arbeitsmappe
                workbook.Save("TotalPagesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


