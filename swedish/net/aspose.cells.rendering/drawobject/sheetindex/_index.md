---
title: "DrawObject.SheetIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DrawObject‑egenskap. Anger aktuellt bladindex för DrawObject"
type: docs
url: /sv/net/aspose.cells.rendering/drawobject/sheetindex/
---
## DrawObject.SheetIndex property

Anger aktuellt bladindex för DrawObject.

```csharp
public int SheetIndex { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    // Anpassad hanterare som läser och visar SheetIndex för varje DrawObject
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
                // Skapa en ny arbetsbok och hämta det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Fyll i några celler för att ha innehåll att rendera
                sheet.Cells["A1"].PutValue("First");
                sheet.Cells["A2"].PutValue("Second");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Lägg till en form så att formens ritobjekt också genereras
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Ställ in renderingsalternativ med vår anpassade hanterare
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new SheetIndexReaderHandler()
                };

                // Rendera kalkylbladet – detta utlöser DrawObject‑händelserna
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "SheetIndexDemo.png");

                // Spara arbetsboken (valfritt)
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

### Se även

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


