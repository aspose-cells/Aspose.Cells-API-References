---
title: "MsoLineFormatHelper.ForeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormatHelper-egenskap. Hämtar och sätter kantlinjens förgrundsfärg"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformathelper/forecolor/
---
## MsoLineFormatHelper.ForeColor property

Hämtar och anger kantlinjens förgrundsfärg.

```csharp
public Color ForeColor { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyForeColorDemo
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

                // Visa det aktuella ForeColor‑värdet
                Console.WriteLine("Current ForeColor: " + lineFormat.ForeColor);

                // Ställ in ett nytt ForeColor (eftersom det är läs/skriv)
                lineFormat.ForeColor = Color.Red;
                Console.WriteLine("Updated ForeColor: " + lineFormat.ForeColor);

                // Visa hur egenskapen påverkar beteendet
                Console.WriteLine("Line fore color has been updated to: " + lineFormat.ForeColor);

                // Spara resultatet
                workbook.Save("ForeColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line fore color.");
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


