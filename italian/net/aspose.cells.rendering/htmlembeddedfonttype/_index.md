---
title: "Enum HtmlEmbeddedFontType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.HtmlEmbeddedFontType enum. Rappresenta il tipo di carattere incorporato in html"
type: docs
url: /it/net/aspose.cells.rendering/htmlembeddedfonttype/
---
## HtmlEmbeddedFontType enumeration

Rappresenta il tipo di font incorporato in HTML.

```csharp
public enum HtmlEmbeddedFontType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Non incorporare il carattere. |
| Woff | `1` | Incorpora il carattere WOFF. |

### Esempi

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
                // Dimostra l'uso dei valori dell'enum HtmlEmbeddedFontType
                HtmlEmbeddedFontType noneType = HtmlEmbeddedFontType.None;
                HtmlEmbeddedFontType woffType = HtmlEmbeddedFontType.Woff;

                // Visualizzare i valori dell'enumerazione
                Console.WriteLine("None font type: " + noneType);
                Console.WriteLine("Woff font type: " + woffType);

                // Dimostra il confronto
                if (noneType == HtmlEmbeddedFontType.None)
                {
                    Console.WriteLine("Font type is correctly set to None");
                }

                if (woffType == HtmlEmbeddedFontType.Woff)
                {
                    Console.WriteLine("Font type is correctly set to Woff");
                }

                // Mostra i valori numerici
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

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


