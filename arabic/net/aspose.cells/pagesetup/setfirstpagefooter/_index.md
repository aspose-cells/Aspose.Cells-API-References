---
title: "PageSetup.SetFirstPageFooter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تقوم بتعيين برنامج نصي ينسق تذييل الصفحة الأولى لملف Excel"
type: docs
url: /ar/net/aspose.cells/pagesetup/setfirstpagefooter/
---
## PageSetup.SetFirstPageFooter method

يضبط برنامجًا نصيًا ينسق تذييل الصفحة الأولى لملف Excel.

```csharp
public void SetFirstPageFooter(int section, string footerScript)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| footerScript | String | نص تنسيق التذييل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFirstPageFooterWithInt32StringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على كائن PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تعيين رؤوس/تذييلات مختلفة للصفحة الأولى
            pageSetup.IsHFDiffFirst = true;
            
            // تعيين تذييل الصفحة الأولى باستخدام فهرس القسم والنص
            pageSetup.SetFirstPageFooter(0, "First Page Footer Text");
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            Console.WriteLine("First page footer set successfully.");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


