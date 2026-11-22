---
title: "Workbook.FileName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل وتعيّن اسم الملف الحالي"
type: docs
url: /ar/net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

يحصل على ويضبط اسم الملف الحالي.

```csharp
public string FileName { get; set; }
```

### ملاحظات

إذا تم فتح الملف عبر تدفق وهناك بعض مراجع الصيغ الخارجية، يرجى تعيين اسم الملف.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // عيّن خاصية اسم الملف
            wb.FileName = "SampleWorkbook.xlsx";
            
            // أضف بعض البيانات لتوضيح الوظيفة
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Workbook FileName Demo");
            sheet.Cells["A2"].PutValue("Current FileName:");
            sheet.Cells["B2"].PutValue(wb.FileName);
            
            // احفظ المصنف
            wb.Save(wb.FileName);
            
            Console.WriteLine($"Workbook created with filename: {wb.FileName}");
            
            // توضيح تغيير اسم الملف
            Workbook wb2 = new Workbook();
            wb2.FileName = "ChangedName.xlsx";
            Console.WriteLine($"New workbook filename set to: {wb2.FileName}");
            
            // توضيح استخدام الرابط الخارجي
            if (wb.Worksheets.ExternalLinks.Count > 0)
            {
                string externalSource = wb.Worksheets.ExternalLinks[0].DataSource;
                wb2.FileName = externalSource;
                Console.WriteLine($"Updated filename to external source: {wb2.FileName}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


