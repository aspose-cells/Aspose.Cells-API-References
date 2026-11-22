---
title: "HtmlSaveOptions.ExportActiveWorksheetOnly"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم تصدير ورقة العمل النشطة فقط إلى ملف html. إذا كان true فسيتم تصدير ورقة العمل النشطة فقط إلى ملف html. إذا كان false فسيتم تصدير المصنف بالكامل إلى ملف html. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

يشير إلى ما إذا كان يتم تصدير ورقة العمل النشطة فقط إلى ملف html. إذا كان true فستُصدر ورقة العمل النشطة فقط إلى ملف html؛ إذا كان false فسيتم تصدير المصنف بالكامل إلى ملف html. القيمة الافتراضية هي false.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportActiveWorksheetOnlyDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد يحتوي على ورقتي عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // إضافة بيانات نموذجية إلى كلتا الورقتين
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // تعيين خيارات حفظ HTML لتصدير ورقة العمل النشطة فقط
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // تعيين ورقة العمل الأولى كالنشطة
            workbook.Worksheets.ActiveSheetIndex = 0;
            
            // حفظ مع ورقة العمل النشطة فقط
            workbook.Save("output_active_sheet_only.html", saveOptions);
            
            // تغيير الورقة النشطة وحفظ مرة أخرى
            workbook.Worksheets.ActiveSheetIndex = 1;
            workbook.Save("output_active_sheet_only2.html", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


