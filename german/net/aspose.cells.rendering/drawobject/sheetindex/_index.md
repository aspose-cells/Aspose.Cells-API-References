---
title: "DrawObject.SheetIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DrawObject‑Eigenschaft. Gibt den aktuellen Blattindex von DrawObject an"
type: docs
url: /de/net/aspose.cells.rendering/drawobject/sheetindex/
---
## DrawObject.SheetIndex property

Gibt den aktuellen Blattindex des DrawObject an.

```csharp
public int SheetIndex { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    // Benutzerdefinierter Handler, der den SheetIndex jedes DrawObject liest und anzeigt
    class SheetIndexReaderHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
            Console.WriteLine($"Page: {drawObject.CurrentPage + 1}/{drawObject.TotalPages}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");
            Console.WriteLine();
        }
    }

    public class DrawObjectPropertySheetIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Füllen Sie einige Zellen, um Inhalte zum Rendern zu haben
                sheet.Cells["A1"].PutValue("First");
                sheet.Cells["A2"].PutValue("Second");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Fügen Sie eine Form hinzu, damit Form‑Zeichnungsobjekte ebenfalls erzeugt werden
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Richten Sie die Rendering‑Optionen mit unserem benutzerdefinierten Handler ein
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new SheetIndexReaderHandler()
                };

                // Rendern Sie das Arbeitsblatt – dies löst die DrawObject‑Ereignisse aus
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "SheetIndexDemo.png");

                // Arbeitsmappe speichern (optional)
                workbook.Save("SheetIndexDemo.xlsx");
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


