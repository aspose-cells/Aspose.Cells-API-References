---
title: "DrawObject.TotalPages"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DrawObject‑egenskap. Anger totalt antal sidor i den aktuella renderingen"
type: docs
url: /sv/net/aspose.cells.rendering/drawobject/totalpages/
---
## DrawObject.TotalPages property

Anger totalt antal sidor i aktuell rendering.

```csharp
public int TotalPages { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyTotalPagesDemo
    {
        // Anpassad handler för att fånga DrawObject‑händelser och läsa TotalPages‑egenskapen
        private class TotalPagesHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Visa värdet för TotalPages‑egenskapen
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
                // Skapa en ny arbetsbok och hämta det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Lägg till exempeldata för att göra renderingen meningsfull
                sheet.Cells["A1"].PutValue("Sample Data");
                sheet.Cells["A2"].PutValue("More Data");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Lägg till en form för att säkerställa att flera draw‑objekt genereras
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Ställ in renderingsalternativ med vår anpassade hanterare
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = false, // Allow multiple pages to demonstrate TotalPages
                    DrawObjectEventHandler = new TotalPagesHandler()
                };

                // Rendera kalkylbladet - detta kommer att utlösa DrawObject‑händelserna
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "TotalPagesDemo.png");

                // Spara arbetsboken
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

### Se även

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


