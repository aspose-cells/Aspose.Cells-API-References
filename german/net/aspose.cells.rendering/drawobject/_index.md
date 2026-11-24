---
title: "Klasse DrawObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.DrawObject‑Klasse. DrawObject wird beim Rendern initialisiert und zurückgegeben"
type: docs
url: /de/net/aspose.cells.rendering/drawobject/
---
## DrawObject class

DrawObject wird beim Rendern initialisiert und zurückgegeben.

```csharp
public class DrawObject
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Cell](../../aspose.cells.rendering/drawobject/cell/) { get; } | Gibt das Cell‑Objekt beim Rendern an. Auf alle Eigenschaften der Zelle kann zugegriffen werden. |
| [CurrentPage](../../aspose.cells.rendering/drawobject/currentpage/) { get; } | Gibt den Seitenindex von DrawObject an. Der Seitenindex beginnt bei Null. Ein Sheet enthält beim Rendern mehrere Seiten. |
| [ImageBytes](../../aspose.cells.rendering/drawobject/imagebytes/) { get; } | Gibt die Bildbytes des gerenderten Diagramms, der Form beim Rendern an. |
| [Shape](../../aspose.cells.rendering/drawobject/shape/) { get; } | Gibt das Shape-Objekt beim Rendern an. Auf alle Eigenschaften der Form kann zugegriffen werden. |
| [SheetIndex](../../aspose.cells.rendering/drawobject/sheetindex/) { get; } | Gibt den aktuellen Blattindex des DrawObject an. |
| [TotalPages](../../aspose.cells.rendering/drawobject/totalpages/) { get; } | Gibt die Gesamtseitenzahl im aktuellen Rendering an. |
| [Type](../../aspose.cells.rendering/drawobject/type/) { get; } | Gibt den Typ des DrawObject an. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;

namespace AsposeCellsExamples
{
    // Benutzerdefinierte Implementierung von DrawObjectEventHandler
    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}");
            Console.WriteLine($"Object Type: {drawObject.Type}");
            Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");

            if (drawObject.Cell != null)
            {
                Console.WriteLine($"Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}");
            }

            if (drawObject.Shape != null)
            {
                Console.WriteLine($"Rendering Shape: {drawObject.Shape.Name}");
            }
        }
    }

    public class DrawObjectDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

            // Eine Form hinzufügen
            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
            shape.Text = "Sample Shape";

            // Eine Instanz von CustomDrawObjectEventHandler erstellen
            CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Bild- oder Druckoptionen festlegen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                DrawObjectEventHandler = drawObjectEventHandler,
                OnePagePerSheet = true,
                ImageType = Aspose.Cells.Drawing.ImageType.Png
            };

            // Das Blatt in ein Bild rendern
            SheetRender sr = new SheetRender(sheet, options);
            sr.ToImage(0, "DrawObjectDemo.png");

            // Speichere die Arbeitsmappe
            workbook.Save("DrawObjectDemo.xlsx");
            workbook.Save("DrawObjectDemo.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


