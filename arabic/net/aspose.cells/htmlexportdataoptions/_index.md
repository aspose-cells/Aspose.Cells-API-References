---
title: "تعداد HtmlExportDataOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.HtmlExportDataOptions. يمثل الخيارات لتصدير بيانات html"
type: docs
url: /ar/net/aspose.cells/htmlexportdataoptions/
---
## HtmlExportDataOptions enumeration

يمثل الخيارات لتصدير بيانات HTML.

```csharp
public enum HtmlExportDataOptions
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Table | `1` | تصدير الملف إلى html يحتوي فقط على جزء الجدول. |
| All | `255` | تصدير جميع البيانات إلى html. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlExportDataOptionsDemo
    {
        public static void HtmlExportDataOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Doe");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء HtmlSaveOptions وتعيين HtmlExportDataOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All; // Export all data to HTML

            // حفظ المصنف بتنسيق HTML
            workbook.Save("HtmlExportDataOptionsExample_All.html", saveOptions);

            // تغيير HtmlExportDataOptions لتصدير جزء الجدول فقط
            saveOptions.ExportDataOptions = HtmlExportDataOptions.Table; // Export only the table part

            // احفظ المصنف بتنسيق HTML مرة أخرى
            workbook.Save("HtmlExportDataOptionsExample_Table.html", saveOptions);

            Console.WriteLine("HTML files have been saved successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


