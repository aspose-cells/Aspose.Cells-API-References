---
title: "ExternalLink.IsVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalLink. تشير إلى ما إذا كان هذا الارتباط الخارجي مرئياً في MS Excel"
type: docs
url: /ar/net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

يشير إلى ما إذا كان هذا الارتباط الخارجي مرئيًا في MS Excel.

```csharp
public bool IsVisible { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف يحتوي على روابط خارجية
            Workbook workbook = new Workbook();
            
            // أضف بعض البيانات إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("External Link Demo");
            
            // إنشاء مصنف جديد لاستخدامه كمصدر للارتباط الخارجي
            Workbook externalWorkbook = new Workbook();
            externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
            externalWorkbook.Save("external_data.xlsx");
            
            // إضافة إشارة إلى ارتباط خارجي
            workbook.Worksheets[0].Cells["B1"].Formula = "='[external_data.xlsx]Sheet1'!A1";
            
            // تحقق من الروابط الخارجية (سيتم إنشاؤها تلقائيًا عند تحميل الصيغ)
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link visibility: {link.IsVisible}");
                Console.WriteLine($"External link data source: {link.DataSource}");
            }
            
            // إنشاء مصنف آخر لتوضيح تحميل ملف موجود
            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("=SUM([example.xls]Sheet1!A1:A10)");
            
            // احفظ وأعد التحميل لتوضيح الروابط الخارجية
            workbook2.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // تحقق من الروابط الخارجية في المصنف المحمّل
            foreach (ExternalLink link in loadedWorkbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link URL: {link.DataSource}, Visible: {link.IsVisible}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


