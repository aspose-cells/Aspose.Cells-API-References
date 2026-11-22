---
title: "PageSetup.GetFirstPageFooter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تحصل على نص ينسق تذييل الصفحة الأولى لملف Excel"
type: docs
url: /ar/net/aspose.cells/pagesetup/getfirstpagefooter/
---
## PageSetup.GetFirstPageFooter method

يحصل على برنامج نصي ينسق تذييل الصفحة الأولى لملف Excel.

```csharp
public string GetFirstPageFooter(int section)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetFirstPageFooterWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين تذييل الصفحة الأولى
            worksheet.PageSetup.SetFirstPageFooter(1, "First Page Footer");

            // الحصول على وتطباعة تذييل الصفحة الأولى
            string footer = worksheet.PageSetup.GetFirstPageFooter(1);
            Console.WriteLine("First Page Footer: " + footer);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


