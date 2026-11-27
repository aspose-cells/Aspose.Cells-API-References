---
title: "DrawObject.Shape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DrawObject‑egenskap. Anger Shape‑objektet vid rendering. Alla egenskaper för shape kan nås"
type: docs
url: /sv/net/aspose.cells.rendering/drawobject/shape/
---
## DrawObject.Shape property

Anger Shape-objektet vid rendering. Alla egenskaper för shape kan nås.

```csharp
public Shape Shape { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyShapeDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok och hämta det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata för att göra renderingen meningsfull
                worksheet.Cells["A1"].Value = "Sample Data";
                worksheet.Cells["A2"].Value = "More Data";

                // Lägg till en form i kalkylbladet
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Ställ in renderingsalternativ med en anpassad hanterare
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new ShapePropertyHandler()
                };

                // Rendera kalkylbladet - detta kommer att utlösa DrawObject‑händelserna
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "ShapeDemo.png");

                // Spara arbetsboken
                workbook.Save("ShapeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Anpassad hanterare för att fånga DrawObject‑händelser och läsa Shape‑egenskapen
        private class ShapePropertyHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                if (drawObject.Shape != null)
                {
                    Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                    Console.WriteLine($"Shape Name: {drawObject.Shape.Name}");
                    Console.WriteLine($"Shape Text: {drawObject.Shape.Text}");
                    Console.WriteLine($"Shape Width: {drawObject.Shape.Width} pixels");
                    Console.WriteLine($"Shape Height: {drawObject.Shape.Height} pixels");
                    Console.WriteLine($"Shape Type: {drawObject.Shape.AutoShapeType}");
                    Console.WriteLine();
                }
            }
        }
    }
}
```

### Se även

* class [Shape](../../../aspose.cells.drawing/shape/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


