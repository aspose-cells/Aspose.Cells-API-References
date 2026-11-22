---
title: "Workbook.Unprotect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تزيل الحماية عن دفتر العمل"
type: docs
url: /ar/net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

يفك حماية مصنف.

```csharp
public void Unprotect(string password)
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
    public class WorkbookMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مع الحماية
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.All, "book");

            // إزالة حماية دفتر العمل باستخدام كلمة المرور الصحيحة
            workbook.Unprotect("book");

            // حفظ دفتر العمل غير المحمي
            workbook.Save("unprotected_workbook.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


