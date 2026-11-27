---
title: "Enum HtmlEmbeddedFontType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.HtmlEmbeddedFontType enum. Representerar den inbäddade typsnittstypen i html"
type: docs
url: /sv/net/aspose.cells.rendering/htmlembeddedfonttype/
---
## HtmlEmbeddedFontType enumeration

Representerar den inbäddade typsnittstypen i HTML.

```csharp
public enum HtmlEmbeddedFontType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Inte bädda in teckensnitt. |
| Woff | `1` | Inbädda WOFF-typsnitt. |

### Exempel

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
                // Demonstrera användning av enum‑värdena för HtmlEmbeddedFontType
                HtmlEmbeddedFontType noneType = HtmlEmbeddedFontType.None;
                HtmlEmbeddedFontType woffType = HtmlEmbeddedFontType.Woff;

                // Visa enum‑värden
                Console.WriteLine("None font type: " + noneType);
                Console.WriteLine("Woff font type: " + woffType);

                // Demonstrera jämförelse
                if (noneType == HtmlEmbeddedFontType.None)
                {
                    Console.WriteLine("Font type is correctly set to None");
                }

                if (woffType == HtmlEmbeddedFontType.Woff)
                {
                    Console.WriteLine("Font type is correctly set to Woff");
                }

                // Visa numeriska värden
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

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


