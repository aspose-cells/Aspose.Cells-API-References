---
title: "ImageOrPrintOptions.GridlineColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions‑egenskap. Hämtar eller anger färg på rutlinjer"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

Hämtar eller anger färg på rutnätslinjer.

```csharp
public Color GridlineColor { get; set; }
```

### Anmärkningar

Den kommer att ignorera inställningarna för rutlinjefärg i källfilen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata så att kalkylbladet har innehåll
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // Skapa en instans av ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visa det aktuella GridlineColor‑värdet (skrivskyddat eller läs/skriv)
                // Egenskapstypen antas vara System.Drawing.Color
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // Rendera eventuellt bladet till en bild för att se effekten av standardfärgen för rutlinjer
                // (Ingen anledning att ändra värdet; vi demonstrerar bara användning.)
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // Spara arbetsboken (valfritt)
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


