---
title: "MsoLineFormatHelper.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormatHelper-egenskap. Returnerar eller sätter transparensgraden för den angivna fyllningen som ett värde från 0,0 (opak) till 1,0 (klar)"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformathelper/transparency/
---
## MsoLineFormatHelper.Transparency property

Returnerar eller anger graden av transparens för den angivna fyllningen som ett värde från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Skapa en form för att demonstrera linjeformatering
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Hämta linjeformatet
                MsoLineFormat lineFormat = shape.LineFormat;

                // Visa det aktuella Transparency‑värdet
                Console.WriteLine("Current Transparency: " + lineFormat.Transparency);

                // Ställ in ett nytt Transparency‑värde (eftersom det är läs/skriv)
                lineFormat.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + lineFormat.Transparency);

                // Visa hur egenskapen påverkar beteendet
                Console.WriteLine("Line transparency has been updated to: " + lineFormat.Transparency);

                // Spara resultatet
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line transparency.");
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

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


