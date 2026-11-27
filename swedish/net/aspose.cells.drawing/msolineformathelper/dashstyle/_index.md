---
title: "MsoLineFormatHelper.DashStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormatHelper egenskap. Hämtar eller anger streckstilen för den angivna linjen"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformathelper/dashstyle/
---
## MsoLineFormatHelper.DashStyle property

Hämtar eller anger streckstilen för den angivna linjen.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyDashStyleDemo
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

                // Visa det aktuella DashStyle‑värdet
                Console.WriteLine("Current DashStyle: " + lineFormat.DashStyle);

                // Ange ett nytt DashStyle‑värde (eftersom det är läs/skriv)
                lineFormat.DashStyle = MsoLineDashStyle.DashDot;
                Console.WriteLine("Updated DashStyle: " + lineFormat.DashStyle);

                // Visa hur egenskapen påverkar beteendet
                Console.WriteLine("Line dash style has been updated to: " + lineFormat.DashStyle);

                // Spara resultatet
                workbook.Save("DashStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line dash style.");
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

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


