---
title: "Enumeración HtmlEmbeddedFontType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Rendering.HtmlEmbeddedFontType. Representa el tipo de fuente incrustada en HTML"
type: docs
url: /es/net/aspose.cells.rendering/htmlembeddedfonttype/
---
## HtmlEmbeddedFontType enumeration

Representa el tipo de fuente incrustada en HTML.

```csharp
public enum HtmlEmbeddedFontType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | No incrustar fuente. |
| Woff | `1` | Incrustar fuente WOFF. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Demostrar el uso de los valores de la enumeración HtmlEmbeddedFontType
                HtmlEmbeddedFontType noneType = HtmlEmbeddedFontType.None;
                HtmlEmbeddedFontType woffType = HtmlEmbeddedFontType.Woff;

                // Mostrar los valores del enum
                Console.WriteLine("None font type: " + noneType);
                Console.WriteLine("Woff font type: " + woffType);

                // Demostrar comparación
                if (noneType == HtmlEmbeddedFontType.None)
                {
                    Console.WriteLine("Font type is correctly set to None");
                }

                if (woffType == HtmlEmbeddedFontType.Woff)
                {
                    Console.WriteLine("Font type is correctly set to Woff");
                }

                // Mostrar valores numéricos
                Console.WriteLine("Numeric value for None: " + (int)noneType);
                Console.WriteLine("Numeric value for Woff: " + (int)woffType);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlEmbeddedFontType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


