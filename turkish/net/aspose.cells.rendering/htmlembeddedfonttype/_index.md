---
title: "Enum HtmlEmbeddedFontType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.HtmlEmbeddedFontType enum. HTML'de gömülü yazı tipi türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.rendering/htmlembeddedfonttype/
---
## HtmlEmbeddedFontType enumeration

HTML'de gömülü yazı tipi türünü temsil eder.

```csharp
public enum HtmlEmbeddedFontType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Yazı tipi gömülmedi. |
| Woff | `1` | WOFF yazı tipini göm. |

### Örnekler

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
                // HtmlEmbeddedFontType enum değerlerini kullanmayı göster
                HtmlEmbeddedFontType noneType = HtmlEmbeddedFontType.None;
                HtmlEmbeddedFontType woffType = HtmlEmbeddedFontType.Woff;

                // Enum değerlerini görüntüle
                Console.WriteLine("None font type: " + noneType);
                Console.WriteLine("Woff font type: " + woffType);

                // Karşılaştırmayı göster
                if (noneType == HtmlEmbeddedFontType.None)
                {
                    Console.WriteLine("Font type is correctly set to None");
                }

                if (woffType == HtmlEmbeddedFontType.Woff)
                {
                    Console.WriteLine("Font type is correctly set to Woff");
                }

                // Sayısal değerleri göster
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


