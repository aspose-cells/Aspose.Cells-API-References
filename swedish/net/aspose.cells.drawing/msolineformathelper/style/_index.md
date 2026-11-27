---
title: "MsoLineFormatHelper.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormatHelper egenskap. Returnerar ett Style‑objekt som representerar stilen för det angivna intervallet"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformathelper/style/
---
## MsoLineFormatHelper.Style property

Returnerar ett Style-objekt som representerar stilen för det angivna intervallet.

```csharp
public MsoLineStyle Style { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyStyleDemo
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

                // Hämta linjeformatet direkt (MsoLineFormatHelper verkar vara en hjälparklass)
                // Eftersom vi inte kan instansiera MsoLineFormatHelper direkt, kommer vi att arbeta med LineFormat‑egenskapen
                MsoLineFormat lineFormat = shape.LineFormat;

                // Visa det aktuella Style‑värdet
                Console.WriteLine("Current Line Style: " + lineFormat.Style);

                // Ange en ny stil (eftersom Style är läs/skriv)
                lineFormat.Style = MsoLineStyle.ThickBetweenThin;
                Console.WriteLine("Updated Line Style: " + lineFormat.Style);

                // Visa hur egenskapen påverkar beteendet
                Console.WriteLine("Line style has been updated to: " + lineFormat.Style);

                // Spara resultatet
                workbook.Save("LineStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line style.");
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

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


