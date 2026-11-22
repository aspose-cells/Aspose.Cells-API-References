---
title: "PageSetup.IsAutoFirstPageNumber"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تشير إلى ما إذا كان رقم الصفحة الأول يُعيّن تلقائيًا"
type: docs
url: /ar/net/aspose.cells/pagesetup/isautofirstpagenumber/
---
## PageSetup.IsAutoFirstPageNumber property

يشير إلى ما إذا كان رقم الصفحة الأولى يُعيّن تلقائيًا.

```csharp
public bool IsAutoFirstPageNumber { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutoFirstPageNumberDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين خصائص إعداد الصفحة
            worksheet.PageSetup.IsAutoFirstPageNumber = true;
            Console.WriteLine("Auto First Page Number (Worksheet 1): " + worksheet.PageSetup.IsAutoFirstPageNumber);

            // إضافة ورقة عمل ثانية
            worksheet = workbook.Worksheets.Add("Sheet2");
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            Console.WriteLine("Auto First Page Number (Worksheet 2): " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("First Page Number (Worksheet 2): " + worksheet.PageSetup.FirstPageNumber);

            // احفظ المصنف
            workbook.Save("PageSetup_IsAutoFirstPageNumber_Example.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


