---
title: "HtmlSaveOptions.HiddenRowDisplayType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. الصف المخفي ارتفاع هذا الصف هو 0 في Excel قبل حفظه بتنسيق html إذا كان HtmlHiddenRowDisplayType هو Remove فلن يتم إخراج الصف المخفي إذا كانت القيمة Hidden سيتم إخراج الصف لكنه مخفي القيمة الافتراضية هي Hidden"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

صف مخفي (ارتفاع هذا الصف هو 0) في Excel، قبل حفظه بصيغة html، إذا كان HtmlHiddenRowDisplayType هو "Remove"، فلن يتم إخراج الصف المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج الصف ولكنه مخفي، القيمة الافتراضية هي "Hidden"

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenRowDisplayTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة وإخفاء صف
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row");
            worksheet.Cells.HideRow(1); // Hide row 2 (0-based index 1)

            // تعيين خيارات حفظ HTML مع HiddenRowDisplayType
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;

            // حفظ إلى HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with hidden rows handled according to HiddenRowDisplayType setting.");
        }
    }
}
```

### انظر أيضًا

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


