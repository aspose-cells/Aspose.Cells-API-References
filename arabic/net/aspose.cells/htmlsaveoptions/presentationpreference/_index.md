---
title: "HtmlSaveOptions.PresentationPreference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "HtmlSaveOptions property. تشير إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا يرجى تعيين القيمة إلى true"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/presentationpreference/
---
## HtmlSaveOptions.PresentationPreference property

يشير إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true.

```csharp
public bool PresentationPreference { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPresentationPreferenceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Presentation Preference Test");
            worksheet.Cells["B1"].PutValue(123.45);
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // تعيين خيارات حفظ HTML مع PresentationPreference
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.PresentationPreference = true;
            options.IsFullPathLink = false;

            // حفظ إلى تدفق الذاكرة للعرض
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                Console.WriteLine("Workbook saved with PresentationPreference=true");
            }
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


