---
title: "MsoLineFormatHelper.Weight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormatHelper egenskap. Returnerar eller anger linjens tjocklek i enheter av pt"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformathelper/weight/
---
## MsoLineFormatHelper.Weight property

Returnerar eller anger linjens tjocklek i enheter av pt.

```csharp
public double Weight { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyWeightDemo
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

                // Visa det aktuella Weight‑värdet
                Console.WriteLine("Current Line Weight: " + lineFormat.Weight);

                // Ange ett nytt Weight‑värde (eftersom det är läs/skriv)
                lineFormat.Weight = 2.5;
                Console.WriteLine("Updated Line Weight: " + lineFormat.Weight);

                // Visa hur egenskapen påverkar beteendet
                Console.WriteLine("Line weight has been updated to: " + lineFormat.Weight);

                // Spara resultatet
                workbook.Save("WeightDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line weight.");
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


