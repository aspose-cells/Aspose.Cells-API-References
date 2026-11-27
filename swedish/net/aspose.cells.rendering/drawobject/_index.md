---
title: "Class DrawObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.DrawObject klass. DrawObject kommer att initieras och returneras vid rendering"
type: docs
url: /sv/net/aspose.cells.rendering/drawobject/
---
## DrawObject class

DrawObject kommer att initieras och returneras vid rendering.

```csharp
public class DrawObject
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Cell](../../aspose.cells.rendering/drawobject/cell/) { get; } | Indikerar Cell‑objektet vid rendering. Alla egenskaper för cellen kan nås. |
| [CurrentPage](../../aspose.cells.rendering/drawobject/currentpage/) { get; } | Indikerar sidindex för DrawObject. Sidindex är nollbaserat. Ett blad innehåller flera sidor vid rendering. |
| [ImageBytes](../../aspose.cells.rendering/drawobject/imagebytes/) { get; } | Anger bildbytes för renderad Chart, Shape vid rendering. |
| [Shape](../../aspose.cells.rendering/drawobject/shape/) { get; } | Anger Shape-objektet vid rendering. Alla egenskaper för shape kan nås. |
| [SheetIndex](../../aspose.cells.rendering/drawobject/sheetindex/) { get; } | Anger aktuellt bladindex för DrawObject. |
| [TotalPages](../../aspose.cells.rendering/drawobject/totalpages/) { get; } | Anger totalt antal sidor i aktuell rendering. |
| [Type](../../aspose.cells.rendering/drawobject/type/) { get; } | Anger typen av DrawObject. |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;

namespace AsposeCellsExamples
{
    // Anpassad implementation av DrawObjectEventHandler
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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

            // Lägg till en shape
            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
            shape.Text = "Sample Shape";

            // Skapa en instans av CustomDrawObjectEventHandler
            CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Ställ in bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                DrawObjectEventHandler = drawObjectEventHandler,
                OnePagePerSheet = true,
                ImageType = Aspose.Cells.Drawing.ImageType.Png
            };

            // Rendera bladet till en bild
            SheetRender sr = new SheetRender(sheet, options);
            sr.ToImage(0, "DrawObjectDemo.png");

            // Spara arbetsboken
            workbook.Save("DrawObjectDemo.xlsx");
            workbook.Save("DrawObjectDemo.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


