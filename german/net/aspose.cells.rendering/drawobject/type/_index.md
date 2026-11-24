---
title: "DrawObject.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DrawObject‑Eigenschaft. Gibt den Typ von DrawObject an"
type: docs
url: /de/net/aspose.cells.rendering/drawobject/type/
---
## DrawObject.Type property

Gibt den Typ des DrawObject an.

```csharp
public DrawObjectEnum Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    public class DrawObjectPropertyTypeDemo
    {
        // Benutzerdefinierter Handler, der die Type‑Eigenschaft jedes DrawObject ausliest und anzeigt
        private class TypeReaderHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}, Page: {drawObject.CurrentPage}/{drawObject.TotalPages}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Füllen Sie einige Zellen
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Fügen Sie ein Shape hinzu, um ebenfalls shape‑Typ‑Draw‑Objekte zu erzeugen
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Legen Sie Rendering‑Optionen mit unserem benutzerdefinierten Draw‑Handler fest
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new TypeReaderHandler()
                };

                // Rendern Sie das Blatt – dies löst die DrawObject‑Ereignisse aus
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectTypeDemo.png");

                // Arbeitsmappe speichern (optional)
                workbook.Save("DrawObjectTypeDemo.xlsx");
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

* enum [DrawObjectEnum](../../drawobjectenum/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


