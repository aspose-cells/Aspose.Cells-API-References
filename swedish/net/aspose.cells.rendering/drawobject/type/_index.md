---
title: "DrawObject.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DrawObject‑egenskap. Anger typen av DrawObject"
type: docs
url: /sv/net/aspose.cells.rendering/drawobject/type/
---
## DrawObject.Type property

Anger typen av DrawObject.

```csharp
public DrawObjectEnum Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    public class DrawObjectPropertyTypeDemo
    {
        // Anpassad hanterare som läser och visar Type‑egenskapen för varje DrawObject
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
                // Skapa en ny arbetsbok och öppna det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Fyll i några celler
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Lägg till en shape för att också generera shape‑typade ritobjekt
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Ställ in renderingsalternativ med vår anpassade ritningshanterare
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new TypeReaderHandler()
                };

                // Rendera bladet – detta utlöser DrawObject‑händelserna
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectTypeDemo.png");

                // Spara arbetsboken (valfritt)
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

### Se även

* enum [DrawObjectEnum](../../drawobjectenum/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


