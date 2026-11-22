---
title: "تعداد HtmlEmbeddedFontType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Rendering.HtmlEmbeddedFontType. يمثل نوع الخط المضمن في html"
type: docs
url: /ar/net/aspose.cells.rendering/htmlembeddedfonttype/
---
## HtmlEmbeddedFontType enumeration

يمثل نوع الخط المدمج في HTML.

```csharp
public enum HtmlEmbeddedFontType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | عدم تضمين الخط. |
| Woff | `1` | تضمين خط WOFF. |

### أمثلة

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
                // عرض استخدام قيم تعداد HtmlEmbeddedFontType
                HtmlEmbeddedFontType noneType = HtmlEmbeddedFontType.None;
                HtmlEmbeddedFontType woffType = HtmlEmbeddedFontType.Woff;

                // عرض قيم التعداد
                Console.WriteLine("None font type: " + noneType);
                Console.WriteLine("Woff font type: " + woffType);

                // عرض المقارنة
                if (noneType == HtmlEmbeddedFontType.None)
                {
                    Console.WriteLine("Font type is correctly set to None");
                }

                if (woffType == HtmlEmbeddedFontType.Woff)
                {
                    Console.WriteLine("Font type is correctly set to Woff");
                }

                // إظهار القيم الرقمية
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

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


