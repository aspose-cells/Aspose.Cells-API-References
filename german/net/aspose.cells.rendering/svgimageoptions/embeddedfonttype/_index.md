---
title: "SvgImageOptions.EmbeddedFontType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SvgImageOptions-Eigenschaft. Gibt den Typ der Schriftart zurück oder legt ihn fest, die in Svg eingebettet ist."
type: docs
url: /de/net/aspose.cells.rendering/svgimageoptions/embeddedfonttype/
---
## SvgImageOptions.EmbeddedFontType property

Liest oder setzt den Typ der Schriftart, die in SVG eingebettet ist.

```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```

### Hinweise

Der Standardwert ist None, was bedeutet, dass keine Schriftart in Svg eingebettet wird.

### Beispiele

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
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten mit benutzerdefinierter Formatierung hinzufügen, um die Schriftarteinbettung zu demonstrieren.
            var cell = worksheet.Cells["B2"];
            cell.PutValue("SVG Font Embedding Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Erstelle SVG-Renderoptionen
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Anfangs eingebetteten Schriftarttyp anzeigen.
            Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");

            // Arbeitsblatt ohne Schriftarteinbettung in SVG rendern.
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "WithoutFontEmbedding.svg");

            // Eingebetteten Schriftarttyp zu WOFF ändern.
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

            // Arbeitsblatt mit WOFF-Schriftarteinbettung in SVG rendern.
            SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
            renderer2.ToImage(0, "WithWoffFontEmbedding.svg");

            Console.WriteLine("Generated SVG files with different font embedding settings.");
        }
    }
}
```

### Siehe auch

* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


