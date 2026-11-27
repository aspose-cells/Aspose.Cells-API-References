---
title: "MsoFillFormatHelper.ForeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormatHelper property. Hämtar och anger fyllningens förgrundsfärg"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformathelper/forecolor/
---
## MsoFillFormatHelper.ForeColor property

Hämtar och anger fyllningens förgrundsfärg.

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
    using System.Reflection;

    public class MsoFillFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en etikett för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "ForeColor Property Demo";

            try
            {
                // Skapa en instans av MsoFillFormatHelper med hjälp av reflektion (ingen publik konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visa standardvärdet för ForeColor
                Console.WriteLine($"Default ForeColor: {fillHelper.ForeColor}");

                // Ange ett nytt ForeColor‑värde
                fillHelper.ForeColor = Color.FromArgb(255, 128, 0, 128); // Purple color
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");

                // Demonstrera hämtning av ForeColor‑värdet
                Color currentColor = fillHelper.ForeColor;
                Console.WriteLine($"Current ForeColor (RGB): R={currentColor.R}, G={currentColor.G}, B={currentColor.B}");

                // Spara arbetsboken för att demonstrera en lyckad körning
                workbook.Save("ForeColorDemo.xlsx");

                Console.WriteLine("ForeColor property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColor demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


