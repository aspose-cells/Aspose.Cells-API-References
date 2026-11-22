---
title: "PageSetup.GetFirstPageHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تحصل على سكريبت ينسق رأس الصفحة الأولى لملف Excel"
type: docs
url: /ar/net/aspose.cells/pagesetup/getfirstpageheader/
---
## PageSetup.GetFirstPageHeader method

يحصل على برنامج نصي ينسق رأس الصفحة الأولى لملف Excel.

```csharp
public string GetFirstPageHeader(int section)
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
    public class PageSetupMethodGetFirstPageHeaderWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تمكين رأس/تذييل مختلف للصفحة الأولى
            pageSetup.IsHFDiffFirst = true;
            
            // تعيين أقسام رأس الصفحة الأولى
            pageSetup.SetFirstPageHeader(0, "&LFirst Page Left Header");
            pageSetup.SetFirstPageHeader(1, "&CFirst Page Center Header");
            pageSetup.SetFirstPageHeader(2, "&RFirst Page Right Header");
            
            // احصل على أقسام رأس الصفحة الأولى وعرضها
            Console.WriteLine("First Page Header Sections:");
            Console.WriteLine("Left: " + pageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Center: " + pageSetup.GetFirstPageHeader(1));
            Console.WriteLine("Right: " + pageSetup.GetFirstPageHeader(2));
            
            // احفظ المصنف
            workbook.Save("PageSetupFirstPageHeaderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


