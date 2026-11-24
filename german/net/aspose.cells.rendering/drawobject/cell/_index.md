---
title: "DrawObject.Cell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DrawObject‑Eigenschaft. Gibt das Cell‑Objekt beim Rendern an. Auf alle Eigenschaften der Zelle kann zugegriffen werden"
type: docs
url: /de/net/aspose.cells.rendering/drawobject/cell/
---
## DrawObject.Cell property

Gibt das Cell‑Objekt beim Rendern an. Auf alle Eigenschaften der Zelle kann zugegriffen werden.

```csharp
public Cell Cell { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    // Benutzerdefinierter Handler zum Erfassen von DrawObject‑Ereignissen und zum Lesen der Cell‑Eigenschaft
    public class CellInfoDrawHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Geben Sie grundlegende Informationen zum Zeichnungsobjekt aus
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");

            // Demonstrieren Sie das Lesen der schreibgeschützten Cell‑Eigenschaft
            if (drawObject.Cell != null)
            {
                var cell = drawObject.Cell;
                Console.WriteLine($"Cell Name: {cell.Name}");
                Console.WriteLine($"Cell Value: {cell.Value}");
                Console.WriteLine($"Cell Row: {cell.Row}, Column: {cell.Column}");
            }
        }
    }

    public class DrawObjectPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Fügen Sie einigen Zellen Beispieldaten hinzu
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Fügen Sie eine Form hinzu, um sicherzustellen, dass Form‑Zeichnungsereignisse ebenfalls ausgelöst werden
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Richten Sie die Rendering‑Optionen mit unserem benutzerdefinierten Zeichen‑Handler ein
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CellInfoDrawHandler()
                };

                // Rendern Sie das Arbeitsblatt – dies wird die DrawObject‑Ereignisse auslösen
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectCellDemo.png");

                // Arbeitsmappe speichern (optional)
                workbook.Save("DrawObjectCellDemo.xlsx");
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

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


