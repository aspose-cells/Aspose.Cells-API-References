---
title: "HtmlSaveOptions.HiddenColDisplayType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. العمود المخفي عرض هذا العمود هو 0 في إكسل قبل حفظه إلى صيغة html إذا كان HtmlHiddenColDisplayType هو Remove فإن العمود المخفي لن يتم إخراجه إذا كانت القيمة Hidden فإن العمود سيتم إخراجه لكنه مخفي القيمة الافتراضية هي Hidden"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/hiddencoldisplaytype/
---
## HtmlSaveOptions.HiddenColDisplayType property

العمود المخفي (عرض هذا العمود هو 0) في Excel، قبل حفظه بصيغة html، إذا كان HtmlHiddenColDisplayType هو \"Remove\"، فلن يتم إخراج العمود المخفي، إذا كانت القيمة \"Hidden\"، سيتم إخراج العمود لكنه سيبقى مخفيًا، القيمة الافتراضية هي \"Hidden\".

```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenColDisplayTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إخفاء العمود C (الفهرس 2)
            worksheet.Cells.HideColumn(2);

            // أضف بعض البيانات للتوضيح
            worksheet.Cells["A1"].PutValue("Visible Column A");
            worksheet.Cells["B1"].PutValue("Visible Column B");
            worksheet.Cells["C1"].PutValue("Hidden Column C");
            worksheet.Cells["D1"].PutValue("Visible Column D");

            // إنشاء خيارات حفظ HTML بإعدادات HiddenColDisplayType مختلفة
            HtmlSaveOptions optionsRemove = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
            };

            HtmlSaveOptions optionsHidden = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden
            };

            // احفظ بإعدادات مختلفة
            workbook.Save("output_remove.html", optionsRemove); // Column C will be removed
            workbook.Save("output_hidden.html", optionsHidden); // Column C will be hidden but space preserved
        }
    }
}
```

### انظر أيضًا

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


