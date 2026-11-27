---
title: "MsoLineFormatHelper.BackColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormatHelper egenskap. Hämtar och anger bakgrundsfärgen för kantlinjen"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformathelper/backcolor/
---
## MsoLineFormatHelper.BackColor property

Hämtar och anger kantlinjens bakgrundsfärg.

```csharp
public Color BackColor { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyBackColorDemo
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

                // Visa det aktuella BackColor‑värdet
                Console.WriteLine("Current BackColor: " + lineFormat.BackColor);

                // Ange ett nytt BackColor‑värde (eftersom det är läs/skriv)
                lineFormat.BackColor = Color.LightBlue;
                Console.WriteLine("Updated BackColor: " + lineFormat.BackColor);

                // Visa hur egenskapen påverkar beteendet
                Console.WriteLine("Line back color has been updated to: " + lineFormat.BackColor);

                // Spara resultatet
                workbook.Save("BackColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line back color.");
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


