---
title: "SvgImageOptions.EmbeddedFontType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SvgImageOptions. Ottiene o imposta il tipo di carattere incorporato in Svg"
type: docs
url: /it/net/aspose.cells.rendering/svgimageoptions/embeddedfonttype/
---
## SvgImageOptions.EmbeddedFontType property

Ottiene o imposta il tipo di font incorporato in SVG.

```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```

### Osservazioni

Il valore predefinito è None, il che indica che non verrà incorporato alcun carattere in Svg.

### Esempi

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
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati con formattazione personalizzata per dimostrare l'incorporamento del carattere
            var cell = worksheet.Cells["B2"];
            cell.PutValue("SVG Font Embedding Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Crea opzioni di rendering SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Visualizza il tipo di carattere incorporato iniziale
            Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");

            // Esegui il rendering del foglio di lavoro in SVG senza incorporare il carattere
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "WithoutFontEmbedding.svg");

            // Modifica il tipo di carattere incorporato in WOFF
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

            // Esegui il rendering del foglio di lavoro in SVG con incorporamento del carattere WOFF
            SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
            renderer2.ToImage(0, "WithWoffFontEmbedding.svg");

            Console.WriteLine("Generated SVG files with different font embedding settings.");
        }
    }
}
```

### Vedi anche

* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


