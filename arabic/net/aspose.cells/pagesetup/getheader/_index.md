---
title: "PageSetup.GetHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. يحصل على سكريبت ينسق ترويسة ملف Excel"
type: docs
url: /ar/net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

يحصل على برنامج نصي ينسق الرأس لملف Excel.

```csharp
public string GetHeader(int section)
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
    public class PageSetupMethodGetHeaderWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين ترويسة للقسم 2
            worksheet.PageSetup.SetHeader(2, "&8Report ID: TEST01\n你好Public");
            
            // احصل على ترويسة القسم 2 واطبعها
            string header = worksheet.PageSetup.GetHeader(2);
            Console.WriteLine("Header for section 2: " + header);
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


