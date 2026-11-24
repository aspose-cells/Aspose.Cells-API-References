---
title: "DrawObject.CurrentPage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DrawObject‑Eigenschaft. Gibt den Seitenindex von DrawObject an. Der Seitenindex beginnt bei Null. Ein Blatt enthält beim Rendern mehrere Seiten"
type: docs
url: /de/net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

Gibt den Seitenindex von DrawObject an. Der Seitenindex beginnt bei Null. Ein Sheet enthält beim Rendern mehrere Seiten.

```csharp
public int CurrentPage { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyCurrentPageDemo
    {
        // Benutzerdefinierter Handler zum Lesen und Anzeigen der CurrentPage‑Eigenschaft
        private class CurrentPageHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Zeigen Sie den Wert der CurrentPage‑Eigenschaft an
                Console.WriteLine($"CurrentPage: {drawObject.CurrentPage}");
                Console.WriteLine($"TotalPages: {drawObject.TotalPages}");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Fügen Sie einige Beispieldaten hinzu, um das Rendering sinnvoll zu machen
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["A2"].PutValue("More Data");
                worksheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Fügen Sie ein Shape hinzu, um shape‑Typ‑Draw‑Objekte zu erzeugen
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Richten Sie die Rendering‑Optionen mit unserem benutzerdefinierten Zeichen‑Handler ein
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CurrentPageHandler()
                };

                // Rendern Sie das Arbeitsblatt, um DrawObject‑Ereignisse auszulösen
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "CurrentPageDemo.png");

                // Speichere die Arbeitsmappe
                workbook.Save("CurrentPageDemo.xlsx");
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


