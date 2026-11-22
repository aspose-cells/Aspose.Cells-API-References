---
title: "HtmlSaveOptions.FormatDataIgnoreColumnWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم عرض جميع البيانات المنسقة للخلية عندما يتجاوز العمود. إذا كانت true يتم تجاهل عرض العمود وتُصدَّر جميع بيانات الخلية. إذا كانت false تُصدَّر البيانات كما في Excel. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/
---
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property

تشير إلى ما إذا كان يتم عرض جميع البيانات المنسقة للخلية عندما يتجاوز العمود. إذا كان true يتم تجاهل عرض العمود وسيتم تصدير جميع بيانات الخلية. إذا كان false سيتم تصدير البيانات كما في Excel. القيمة الافتراضية هي false.

```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين بيانات عينة وعرض العمود
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // عرض خاصية FormatDataIgnoreColumnWidth
            saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
            
            // احفظ بإعدادات مختلفة لإظهار التأثير
            workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
            
            saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
            workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


