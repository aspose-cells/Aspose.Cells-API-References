---
title: "Klassen MsoLineFormatHelper"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoLineFormatHelper klass. Representerar linje- och pilspetsformatering"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformathelper/
---
## MsoLineFormatHelper class

Representerar linje- och pilspetsformat.

```csharp
public class MsoLineFormatHelper
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformathelper/backcolor/) { get; set; } | Hämtar och anger kantlinjens bakgrundsfärg. |
| [DashStyle](../../aspose.cells.drawing/msolineformathelper/dashstyle/) { get; set; } | Hämtar eller anger streckstilen för den angivna linjen. |
| [ForeColor](../../aspose.cells.drawing/msolineformathelper/forecolor/) { get; set; } | Hämtar och anger kantlinjens förgrundsfärg. |
| [IsVisible](../../aspose.cells.drawing/msolineformathelper/isvisible/) { get; set; } | Anger om objektet är synligt. |
| [Style](../../aspose.cells.drawing/msolineformathelper/style/) { get; set; } | Returnerar ett Style-objekt som representerar stilen för det angivna intervallet. |
| [Transparency](../../aspose.cells.drawing/msolineformathelper/transparency/) { get; set; } | Returnerar eller anger graden av transparens för den angivna fyllningen som ett värde från 0,0 (opak) till 1,0 (klar). |
| [Weight](../../aspose.cells.drawing/msolineformathelper/weight/) { get; set; } | Returnerar eller anger linjens tjocklek i enheter av pt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en form för att demonstrera linjeformatering
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Hämta linjeformatet direkt från formen
                MsoLineFormat lineFormat = shape.LineFormat;

                // Ange egenskaper direkt på linjeformatet
                lineFormat.IsVisible = true;
                lineFormat.Style = MsoLineStyle.Single;
                lineFormat.ForeColor = Color.Blue;
                lineFormat.BackColor = Color.LightGray;
                lineFormat.DashStyle = MsoLineDashStyle.Solid;
                lineFormat.Transparency = 0.2;
                lineFormat.Weight = 2.5;

                // Visa de konfigurerade egenskaperna
                Console.WriteLine($"Line is visible: {lineFormat.IsVisible}");
                Console.WriteLine($"Line style: {lineFormat.Style}");
                Console.WriteLine($"Fore color: {lineFormat.ForeColor}");
                Console.WriteLine($"Back color: {lineFormat.BackColor}");
                Console.WriteLine($"Dash style: {lineFormat.DashStyle}");
                Console.WriteLine($"Transparency: {lineFormat.Transparency}");
                Console.WriteLine($"Weight: {lineFormat.Weight}");

                // Spara arbetsboken
                workbook.Save("MsoLineFormatHelperDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MsoLineFormatHelper: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


