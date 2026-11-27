---
title: "Line.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Linjeegenskap. Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 ogenomskinlig till 1.0 klar"
type: docs
url: /sv/net/aspose.cells.drawing/line/transparency/
---
## Line.Transparency property

Returnerar eller anger transparensgraden för linjen som ett värde från 0.0 (opak) till 1.0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Lägg till ett linjediagram för att demonstrera linjeegenskaper
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Hämta linjeegenskaperna från diagramseriens kant
                Line line = chart.NSeries[0].Border;

                // Visa det aktuella Transparency‑värdet
                Console.WriteLine("Current Transparency: " + line.Transparency);

                // Ställ in ett nytt Transparency‑värde (0.0 = ogenomskinlig, 1.0 = klar)
                line.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + line.Transparency);

                // Spara arbetsboken
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("Transparency property demonstrated successfully.");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


