---
title: "HtmlSaveOptions.ExportWorksheetProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم تصدير خصائص ورقة العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel يرجى الحفاظ على القيمة الافتراضية"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportworksheetproperties/
---
## HtmlSaveOptions.ExportWorksheetProperties property

تشير إلى ما إذا كان يتم تصدير خصائص ورقة العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

```csharp
public bool ExportWorksheetProperties { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetPropertiesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // تعيين خيارات حفظ HTML مع تعطيل ExportWorksheetProperties
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportWorksheetProperties = false;
            
            // حفظ مع تعطيل خصائص ورقة العمل
            workbook.Save("output_without_worksheet_props.html", options);

            // تمكين تصدير خصائص ورقة العمل
            options.ExportWorksheetProperties = true;
            
            // حفظ مع تمكين خصائص ورقة العمل
            workbook.Save("output_with_worksheet_props.html", options);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


