---
title: "MsoLineFormatHelper.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormatHelper egenskap. Anger om objektet är synligt"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformathelper/isvisible/
---
## MsoLineFormatHelper.IsVisible property

Anger om objektet är synligt.

```csharp
public bool IsVisible { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyIsVisibleDemo
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

                // Visa det aktuella IsVisible‑värdet
                Console.WriteLine("Current IsVisible: " + lineFormat.IsVisible);

                // Ange ett nytt IsVisible‑värde (eftersom det är läs/skriv)
                lineFormat.IsVisible = false;
                Console.WriteLine("Updated IsVisible: " + lineFormat.IsVisible);

                // Visa hur egenskapen påverkar beteendet
                Console.WriteLine("Line visibility has been updated to: " + lineFormat.IsVisible);

                // Spara resultatet
                workbook.Save("IsVisibleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line visibility.");
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


