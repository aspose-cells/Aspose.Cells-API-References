---
title: "Enum HtmlLayoutMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.HtmlLayoutMode-enum. Representerar layoutläget för HTML-rendering"
type: docs
url: /sv/net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

Representerar layoutläget för HTML‑rendering.

```csharp
public enum HtmlLayoutMode
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Normal | `0` | Renderar innehåll som MS Excel. |
| Print | `1` | Renderar innehåll i utskriftslayoutläge. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till lite exempeldata i kalkylbladet
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // Skapa HtmlSaveOptions och sätt layoutläget till Normal
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // Spara arbetsboken med normalt layoutläge
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // Ändra layoutläge till Print
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // Spara arbetsboken med utskriftslayoutläge
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // Visa enum‑värden
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


