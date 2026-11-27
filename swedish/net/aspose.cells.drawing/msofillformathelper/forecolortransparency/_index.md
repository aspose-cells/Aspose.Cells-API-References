---
title: "MsoFillFormatHelper.ForeColorTransparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormatHelper property. Returnerar eller anger graden av förgrundsfärg för den angivna fyllningen som ett värde från 0.0 ogenomskinlig till 1.0 klar"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformathelper/forecolortransparency/
---
## MsoFillFormatHelper.ForeColorTransparency property

Returnerar eller anger graden av förgrundsfärg för den angivna fyllningen som ett värde från 0,0 (opak) till 1,0 (transparent).

```csharp
public double ForeColorTransparency { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en etikett för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "ForeColorTransparency Demo";

            try
            {
                // Skapa en instans av MsoFillFormatHelper med hjälp av reflektion (ingen publik konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visa standardvärdet för ForeColorTransparency
                Console.WriteLine($"Default ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Ange en ny ForeColor och ForeColorTransparency
                fillHelper.ForeColor = Color.Blue;
                fillHelper.ForeColorTransparency = 0.5; // 50% transparency

                // Visa de uppdaterade värdena
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"Updated ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Demonstrera läsning av transparensvärdet
                double transparency = fillHelper.ForeColorTransparency;
                Console.WriteLine($"Current transparency level: {transparency} (0.0=opaque, 1.0=clear)");

                // Spara arbetsboken för att demonstrera en lyckad körning
                workbook.Save("ForeColorTransparencyDemo.xlsx");

                Console.WriteLine("ForeColorTransparency property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColorTransparency demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


