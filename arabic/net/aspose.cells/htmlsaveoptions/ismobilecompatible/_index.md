---
title: "HtmlSaveOptions.IsMobileCompatible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/ismobilecompatible/
---
## HtmlSaveOptions.IsMobileCompatible property

يشير إلى ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. القيمة الافتراضية هي false.

```csharp
public bool IsMobileCompatible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // تعيين التوافق مع الأجهزة المحمولة
            saveOptions.IsMobileCompatible = true;

            // حفظ مع تمكين التوافق مع الأجهزة المحمولة
            workbook.Save("MobileCompatible.html", saveOptions);

            // تغيير إلى غير متوافق مع الأجهزة المحمولة
            saveOptions.IsMobileCompatible = false;
            workbook.Save("NonMobileCompatible.html", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


