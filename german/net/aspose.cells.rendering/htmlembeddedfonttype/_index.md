---
title: "Enum HtmlEmbeddedFontType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.HtmlEmbeddedFontType enum. Stellt den eingebetteten Schriftarttyp in HTML dar"
type: docs
url: /de/net/aspose.cells.rendering/htmlembeddedfonttype/
---
## HtmlEmbeddedFontType enumeration

Stellt den eingebetteten Schriftarttyp in HTML dar.

```csharp
public enum HtmlEmbeddedFontType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Schriftart nicht einbetten. |
| Woff | `1` | WOFF-Schrift einbetten. |

### Beispiele

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
                // Demonstriere die Verwendung der HtmlEmbeddedFontType-Enum-Werte
                HtmlEmbeddedFontType noneType = HtmlEmbeddedFontType.None;
                HtmlEmbeddedFontType woffType = HtmlEmbeddedFontType.Woff;

                // Die Enum-Werte anzeigen
                Console.WriteLine("None font type: " + noneType);
                Console.WriteLine("Woff font type: " + woffType);

                // Vergleich demonstrieren
                if (noneType == HtmlEmbeddedFontType.None)
                {
                    Console.WriteLine("Font type is correctly set to None");
                }

                if (woffType == HtmlEmbeddedFontType.Woff)
                {
                    Console.WriteLine("Font type is correctly set to Woff");
                }

                // Numerische Werte anzeigen
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

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


