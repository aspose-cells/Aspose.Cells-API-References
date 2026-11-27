---
title: "DrawObject.CurrentPage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DrawObject‑egenskap. Anger sidindex för DrawObject. Sidindexet är baserat på noll. Ett blad innehåller flera sidor vid rendering"
type: docs
url: /sv/net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

Indikerar sidindex för DrawObject. Sidindex är nollbaserat. Ett blad innehåller flera sidor vid rendering.

```csharp
public int CurrentPage { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyCurrentPageDemo
    {
        // Anpassad hanterare för att läsa och visa CurrentPage‑egenskapen
        private class CurrentPageHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Visa värdet för CurrentPage‑egenskapen
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
                // Skapa en ny arbetsbok och öppna det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till lite exempeldata för att göra renderingen meningsfull
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["A2"].PutValue("More Data");
                worksheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Lägg till en shape för att generera shape‑typade ritobjekt
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Ställ in renderingsalternativ med vår anpassade ritningshanterare
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CurrentPageHandler()
                };

                // Rendera kalkylbladet för att utlösa DrawObject‑händelser
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "CurrentPageDemo.png");

                // Spara arbetsboken
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

### Se även

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


