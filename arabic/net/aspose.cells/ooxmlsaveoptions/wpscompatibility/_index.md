---
title: "OoxmlSaveOptions.WpsCompatibility"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OoxmlSaveOptions. تشير إلى ما إذا كان يجب جعل ملف xls أكثر توافقًا مع WPS"
type: docs
url: /ar/net/aspose.cells/ooxmlsaveoptions/wpscompatibility/
---
## OoxmlSaveOptions.WpsCompatibility property

تشير إلى ما إذا كان يجب جعل ملف xls أكثر توافقًا مع WPS.

```csharp
[Obsolete("Use WorkbookSetting.WpsCompatibility property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool WpsCompatibility { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية WorkbookSetting.WpsCompatibility. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            
            // إنشاء خيارات حفظ OOXML وتمكين توافق WPS
            OoxmlSaveOptions options = new OoxmlSaveOptions();
            options.WpsCompatibility = true;
            
            // حفظ المصنف مع توافق WPS
            workbook.Save("output_with_wps_compatibility.xlsx", options);
            
            Console.WriteLine("Workbook saved with WPS compatibility enabled.");
        }
    }
}
```

### انظر أيضًا

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


