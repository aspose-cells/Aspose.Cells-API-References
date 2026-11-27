---
title: "Klass MsoFillFormatHelper"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoFillFormatHelper‑klass. Representerar fyllningsformatering för en form"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformathelper/
---
## MsoFillFormatHelper class

Representerar fyllningsformat för en form.

```csharp
public class MsoFillFormatHelper
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformathelper/backcolor/) { get; set; } | Hämtar och anger filens bakgrundsfärg. |
| [ForeColor](../../aspose.cells.drawing/msofillformathelper/forecolor/) { get; set; } | Hämtar och anger fyllningens förgrundsfärg. |
| [ForeColorTransparency](../../aspose.cells.drawing/msofillformathelper/forecolortransparency/) { get; set; } | Returnerar eller anger graden av förgrundsfärg för den angivna fyllningen som ett värde från 0,0 (opak) till 1,0 (transparent). |
| [ImageData](../../aspose.cells.drawing/msofillformathelper/imagedata/) { get; set; } | Hämtar och anger textur‑ och bildfyllnadsdata. |
| [IsVisible](../../aspose.cells.drawing/msofillformathelper/isvisible/) { get; set; } | Indikerar om det finns fyllning. |
| [Texture](../../aspose.cells.drawing/msofillformathelper/texture/) { get; } | Hämtar typen av texturfyllning. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformathelper/setonecolorgradient/)(Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en enfärgsgradient. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.Reflection;

    public class DrawingClassMsoFillFormatHelperDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "MsoFillFormatHelper Demo";

            try
            {
                // Skapa en instans av MsoFillFormatHelper med hjälp av reflektion
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Ställ in grundläggande egenskaper
                fillHelper.ForeColor = Color.FromArgb(255, 100, 150, 200);
                fillHelper.ForeColorTransparency = 0.3;
                fillHelper.BackColor = Color.LightGray;
                fillHelper.IsVisible = true;

                // Visa egenskapsvärden
                Console.WriteLine($"ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency: {fillHelper.ForeColorTransparency}");
                Console.WriteLine($"BackColor: {fillHelper.BackColor}");
                Console.WriteLine($"IsVisible: {fillHelper.IsVisible}");
                Console.WriteLine($"Texture (read-only): {fillHelper.Texture}");

                // Spara arbetsboken
                workbook.Save("MsoFillFormatHelperDemo.xlsx");
                Console.WriteLine("MsoFillFormatHelper demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in MsoFillFormatHelper demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


