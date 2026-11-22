---
title: "Workbook.ProtectSharedWorkbook"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تحمي دفتر عمل مشترك"
type: docs
url: /ar/net/aspose.cells/workbook/protectsharedworkbook/
---
## Workbook.ProtectSharedWorkbook method

يحمي مصنفًا مشتركًا.

```csharp
public void ProtectSharedWorkbook(string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| كلمة المرور | String | كلمة المرور لحماية دفتر العمل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // حماية دفتر العمل المشترك بكلمة مرور
            wb.ProtectSharedWorkbook("abcd");
            
            // حفظ دفتر العمل المحمي
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // تحميل دفتر العمل المحمي
            Workbook wbProtected = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // التحقق من حالة الحماية
            Console.WriteLine("Workbook is protected: " + wbProtected.Settings.IsProtected);
            
            // إلغاء حماية دفتر العمل
            wbProtected.UnprotectSharedWorkbook("abcd");
            
            // حفظ دفتر العمل غير المحمي
            wbProtected.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


