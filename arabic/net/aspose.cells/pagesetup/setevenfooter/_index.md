---
title: "PageSetup.SetEvenFooter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تعيين نص برمجي لتنسيق تذييل الصفحات الزوجية في ملف Excel. لها تأثير فقط في Excel 2007 عندما تكون IsHFDiffOddEven true"
type: docs
url: /ar/net/aspose.cells/pagesetup/setevenfooter/
---
## PageSetup.SetEvenFooter method

يضبط برنامجًا نصيًا ينسق تذييل الصفحة الزوجية لملف Excel. له تأثير فقط في Excel 2007 عندما تكون IsHFDiffOddEven صحيحة.

```csharp
public void SetEvenFooter(int section, string footerScript)
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
    public class PageSetupMethodSetEvenFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // فعّل رؤوس/تذييلات مختلفة للصفحة الأولى والصفحات الزوجية
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;

            // عيّن أنواع تذييل مختلفة
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetFirstPageFooter(0, "First Page Footer");

            // احفظ المصنف
            workbook.Save("PageSetup_SetEvenFooter_Example.xlsx");

            Console.WriteLine("Workbook saved with even page footer set successfully.");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


