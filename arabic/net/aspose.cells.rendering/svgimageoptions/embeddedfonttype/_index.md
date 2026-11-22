---
title: "SvgImageOptions.EmbeddedFontType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SvgImageOptions. يحصل أو يحدد نوع الخط المضمن في Svg"
type: docs
url: /ar/net/aspose.cells.rendering/svgimageoptions/embeddedfonttype/
---
## SvgImageOptions.EmbeddedFontType property

يحصل أو يضبط نوع الخط المضمن في SVG.

```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```

### ملاحظات

القيمة الافتراضية هي None مما يعني أنه لن يتم تضمين الخط في Svg.

### أمثلة

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
            // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات بتنسيق مخصص لإظهار تضمين الخط
            var cell = worksheet.Cells["B2"];
            cell.PutValue("SVG Font Embedding Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // إنشاء خيارات عرض SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // عرض نوع الخط المضمن الأولي
            Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");

            // عرض ورقة العمل كـ SVG دون تضمين الخط
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "WithoutFontEmbedding.svg");

            // تغيير نوع الخط المضمن إلى WOFF
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

            // عرض ورقة العمل كـ SVG مع تضمين خط WOFF
            SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
            renderer2.ToImage(0, "WithWoffFontEmbedding.svg");

            Console.WriteLine("Generated SVG files with different font embedding settings.");
        }
    }
}
```

### انظر أيضًا

* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


