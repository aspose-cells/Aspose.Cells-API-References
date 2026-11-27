---
title: "SvgImageOptions.EmbeddedFontType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SvgImageOptions-egenskap. Hämtar eller anger typen av teckensnitt som är inbäddad i SVG"
type: docs
url: /sv/net/aspose.cells.rendering/svgimageoptions/embeddedfonttype/
---
## SvgImageOptions.EmbeddedFontType property

Hämtar eller anger typen av teckensnitt som är inbäddat i Svg.

```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```

### Anmärkningar

Standardvärdet är None vilket indikerar att det inte kommer att bädda in teckensnitt i SVG.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data med anpassad formatering för att demonstrera teckensnittsinbäddning
            var cell = worksheet.Cells["B2"];
            cell.PutValue("SVG Font Embedding Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Skapa SVG-renderingsalternativ
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Visa initial inbäddad teckensnittstyp
            Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");

            // Rendera kalkylblad till SVG utan teckensnittsinbäddning
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "WithoutFontEmbedding.svg");

            // Ändra inbäddad teckensnittstyp till WOFF
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

            // Rendera kalkylblad till SVG med WOFF-teckensnittsinbäddning
            SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
            renderer2.ToImage(0, "WithWoffFontEmbedding.svg");

            Console.WriteLine("Generated SVG files with different font embedding settings.");
        }
    }
}
```

### Se även

* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


