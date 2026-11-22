---
title: "HtmlSaveOptions.MergeEmptyTdForcely"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان سيتم دمج عنصر TD فارغ بالقوة عند تصدير الملف إلى html. سيقل حجم ملف html بشكل كبير بعد ضبط القيمة إلى true. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى excel أو تصدير خطوط الشبكة المثالية عند حفظ الملف إلى html يرجى الحفاظ على القيمة الافتراضية"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/mergeemptytdforcely/
---
## HtmlSaveOptions.MergeEmptyTdForcely property

تشير إلى ما إذا كان سيتم دمج عنصر TD فارغ بالقوة عند تصدير الملف إلى html. سيقل حجم ملف html بشكل كبير بعد ضبط القيمة إلى true. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى excel أو تصدير خطوط الشبكة المثالية عند حفظ الملف إلى html، يرجى الحفاظ على القيمة الافتراضية.

```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdForcelyDemo
    {
        public static void Run()
        {
            // إنشاء مصنف عينة يحتوي على خلايا فارغة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء بعض الخلايا الفارغة في ورقة العمل
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            // تم ترك B2 فارغًا عمدًا
            
            // حفظ مع تمكين MergeEmptyTdForcely
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.MergeEmptyTdForcely = true;
            workbook.Save("output_with_merge.html", options);
            
            // حفظ بدون MergeEmptyTdForcely للمقارنة
            options.MergeEmptyTdForcely = false;
            workbook.Save("output_without_merge.html", options);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


