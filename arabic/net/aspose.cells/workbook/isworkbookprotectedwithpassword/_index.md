---
title: "Workbook.IsWorkbookProtectedWithPassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تشير إلى ما إذا كان الهيكل أو النافذة محميًا بكلمة مرور"
type: docs
url: /ar/net/aspose.cells/workbook/isworkbookprotectedwithpassword/
---
## Workbook.IsWorkbookProtectedWithPassword property

يشير إلى ما إذا كان الهيكل أو النافذة محميًا بكلمة مرور.

```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsWorkbookProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // إنشاء نسخة جديدة من Workbook
            Workbook workbook = new Workbook();

            // تحقق مما إذا كان دفتر العمل محميًا بكلمة مرور (يجب أن يكون false لدفتر العمل الجديد)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // حماية المصنف باستخدام كلمة مرور
            workbook.Protect(ProtectionType.All, "password123");

            // التحقق الآن مرة أخرى (يجب أن يكون true)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // إلغاء حماية دفتر العمل
            workbook.Unprotect("password123");

            // التحقق النهائي (يجب أن يكون false مرة أخرى)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // تخلص من المصنف
            workbook.Dispose();
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


