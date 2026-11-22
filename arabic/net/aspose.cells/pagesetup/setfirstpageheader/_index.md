---
title: "PageSetup.SetFirstPageHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تقوم بتعيين برنامج نصي ينسق رأس الصفحة الأولى لملف Excel. لها تأثير فقط في Excel 2007 عندما تكون IsHFDiffFirst صحيحة"
type: docs
url: /ar/net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

يضبط تنسيق برنامج نصي لترويسة الصفحة الأولى لملف Excel. يؤثر فقط في Excel 2007 عندما تكون قيمة IsHFDiffFirst صحيحة.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
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
    public class PageSetupMethodSetFirstPageHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // تعيين رأس الصفحة الأولى باستخدام رقم القسم ونص الرأس
            pageSetup.SetFirstPageHeader(2, "&CHeader Text");

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


