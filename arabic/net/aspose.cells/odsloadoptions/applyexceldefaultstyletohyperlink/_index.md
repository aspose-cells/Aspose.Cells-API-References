---
title: "OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsLoadOptions. تشير إلى ما إذا كان يتم تطبيق النمط الافتراضي لبرنامج Excel على الارتباط التشعبي"
type: docs
url: /ar/net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

يشير إلى ما إذا كان سيتم تطبيق النمط الافتراضي لبرنامج Excel على الرابط التشعبي.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyApplyExcelDefaultStyleToHyperlinkDemo
    {
        public static void Run()
        {
            // إنشاء نسخة من OdsLoadOptions
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // عيّن خاصية ApplyExcelDefaultStyleToHyperlink
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            // تحميل ملف ODS باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("sample.ods", loadOptions);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف ارتباطًا تشعبيًا لإظهار تطبيق النمط
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // حفظ دفتر العمل إلى ملف جديد
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


