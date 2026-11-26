---
title: "SvgImageOptions.EmbeddedFontType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SvgImageOptions. Obtiene o establece el tipo de fuente que se incrusta en Svg"
type: docs
url: /es/net/aspose.cells.rendering/svgimageoptions/embeddedfonttype/
---
## SvgImageOptions.EmbeddedFontType property

Obtiene o establece el tipo de fuente que se incrusta en SVG.

```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```

### Observaciones

El valor predeterminado es None, lo que indica que no incrustará la fuente en Svg.

### Ejemplos

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
            // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos con formato personalizado para demostrar la incrustación de fuentes
            var cell = worksheet.Cells["B2"];
            cell.PutValue("SVG Font Embedding Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Crear opciones de renderizado SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Mostrar tipo de fuente incrustada inicial
            Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");

            // Renderizar la hoja de cálculo a SVG sin incrustar fuentes
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "WithoutFontEmbedding.svg");

            // Cambiar el tipo de fuente incrustada a WOFF
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

            // Renderizar la hoja de cálculo a SVG con incrustación de fuente WOFF
            SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
            renderer2.ToImage(0, "WithWoffFontEmbedding.svg");

            Console.WriteLine("Generated SVG files with different font embedding settings.");
        }
    }
}
```

### Ver también

* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


