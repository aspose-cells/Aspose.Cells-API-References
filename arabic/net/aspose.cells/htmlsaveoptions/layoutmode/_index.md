---
title: "HtmlSaveOptions.LayoutMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تحصل أو تعيين وضع التخطيط عند الحفظ إلى HTML. القيمة الافتراضية هي Normal"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

يحصل أو يضبط وضع التخطيط عند الحفظ إلى HTML. القيمة الافتراضية هي Normal

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // إنشاء كائن HtmlSaveOptions
                HtmlSaveOptions options = new HtmlSaveOptions();

                // عرض قيمة LayoutMode الحالية
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // تعيين LayoutMode إلى Print
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // حفظ المصنف بوضع تخطيط Print
                workbook.Save("LayoutModePrint.html", options);

                // تعيين LayoutMode إلى Normal
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // حفظ المصنف بوضع تخطيط Normal
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


