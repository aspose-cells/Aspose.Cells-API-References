---
title: "PageSetup.SetEvenHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تقوم بتعيين برنامج نصي ينسق رأس الصفحة الزوجية لملف Excel. لها تأثير فقط في Excel 2007 عندما تكون IsHFDiffOddEven صحيحة"
type: docs
url: /ar/net/aspose.cells/pagesetup/setevenheader/
---
## PageSetup.SetEvenHeader method

يضبط برنامجًا نصيًا ينسق رأس الصفحة الزوجية لملف Excel. له تأثير فقط في Excel 2007 عندما تكون IsHFDiffOddEven صحيحة.

```csharp
public void SetEvenHeader(int section, string headerScript)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| headerScript | String | نص تنسيق الرأس. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // تمكين رؤوس/تذييلات مختلفة للصفحات الفردية والزوجية
            pageSetup.IsHFDiffOddEven = true;

            // تعيين رأس الصفحة الزوجية باستخدام فهرس القسم والنص
            pageSetup.SetEvenHeader(1, "Even Page Header - Center Section");
            pageSetup.SetEvenHeader(0, "Even Page Header - Left Section");
            pageSetup.SetEvenHeader(2, "Even Page Header - Right Section");

            // احفظ المصنف
            workbook.Save("PageSetup_SetEvenHeaderExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


