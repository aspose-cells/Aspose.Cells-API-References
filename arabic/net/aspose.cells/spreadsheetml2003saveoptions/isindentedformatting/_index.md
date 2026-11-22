---
title: "SpreadsheetML2003SaveOptions.IsIndentedFormatting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SpreadsheetML2003SaveOptions. تتسبب في إزاحة العناصر الفرعية"
type: docs
url: /ar/net/aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/
---
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property

يتسبب في إزاحة العناصر الفرعية.

```csharp
public bool IsIndentedFormatting { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true. إذا كانت القيمة false، فإنها ستقلل من حجم ملف xml

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyIsIndentedFormattingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // قم بتكوين خيارات الحفظ باستخدام تنسيق مُزاح
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions
            {
                IsIndentedFormatting = true
            };

            // احفظ باستخدام تنسيق XML مُزاح
            workbook.Save("output_indented.xml", saveOptions);

            // احفظ بدون تنسيق مُزاح للمقارنة
            saveOptions.IsIndentedFormatting = false;
            workbook.Save("output_not_indented.xml", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


