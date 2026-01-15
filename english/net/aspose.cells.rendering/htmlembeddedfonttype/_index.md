---
title: Enum HtmlEmbeddedFontType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.HtmlEmbeddedFontType enum. Represents the embedded font type in html
type: docs
url: /net/aspose.cells.rendering/htmlembeddedfonttype/
---
## HtmlEmbeddedFontType enumeration

Represents the embedded font type in html.

```csharp
public enum HtmlEmbeddedFontType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Not embed font. |
| Woff | `1` | Embed WOFF font. |

### Examples

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
                // Demonstrate using the HtmlEmbeddedFontType enum values
                HtmlEmbeddedFontType noneType = HtmlEmbeddedFontType.None;
                HtmlEmbeddedFontType woffType = HtmlEmbeddedFontType.Woff;

                // Display the enum values
                Console.WriteLine("None font type: " + noneType);
                Console.WriteLine("Woff font type: " + woffType);

                // Demonstrate comparison
                if (noneType == HtmlEmbeddedFontType.None)
                {
                    Console.WriteLine("Font type is correctly set to None");
                }

                if (woffType == HtmlEmbeddedFontType.Woff)
                {
                    Console.WriteLine("Font type is correctly set to Woff");
                }

                // Show numeric values
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

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


