---
title: "DrawObject.Cell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DrawObject‑egenskap. Anger Cell‑objektet vid rendering. Alla egenskaper för cellen kan nås"
type: docs
url: /sv/net/aspose.cells.rendering/drawobject/cell/
---
## DrawObject.Cell property

Indikerar Cell‑objektet vid rendering. Alla egenskaper för cellen kan nås.

```csharp
public Cell Cell { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    // Anpassad hanterare för att fånga DrawObject‑händelser och läsa Cell‑egenskapen
    public class CellInfoDrawHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Skriv ut grundläggande information om ritobjektet
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");

            // Demonstrera läsning av den skrivskyddade Cell‑egenskapen
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
                // Skapa en ny arbetsbok och hämta det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Lägg till lite exempeldata i celler
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Lägg till en form för att säkerställa att formrit‑händelser också utlöses
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Ställ in renderingsalternativ med vår anpassade ritningshanterare
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CellInfoDrawHandler()
                };

                // Rendera kalkylbladet – detta kommer att utlösa DrawObject‑händelserna
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectCellDemo.png");

                // Spara arbetsboken (valfritt)
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

### Se även

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


