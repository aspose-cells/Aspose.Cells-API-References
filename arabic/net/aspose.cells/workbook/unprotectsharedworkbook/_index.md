---
title: "Workbook.UnprotectSharedWorkbook"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تُزيل الحماية عن دفتر عمل مشترك"
type: docs
url: /ar/net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

يفك حماية مصنف مشترك.

```csharp
public void UnprotectSharedWorkbook(string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| كلمة المرور | String | كلمة المرور لإزالة حماية دفتر العمل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // حماية دفتر العمل المشترك بكلمة مرور
            wb.ProtectSharedWorkbook("abcd");
            
            // حفظ دفتر العمل المحمي
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // أعد فتح المصنف
            wb = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // إزالة الحماية عن دفتر العمل المشترك باستخدام كلمة مرور
            wb.UnprotectSharedWorkbook("abcd");
            
            // حفظ دفتر العمل غير المحمي
            wb.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


