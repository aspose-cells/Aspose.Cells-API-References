---
title: "ProtectedRange.IsProtectedWithPassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ProtectedRange. تشير إلى ما إذا كان ورقة العمل محمية بكلمة مرور"
type: docs
url: /ar/net/aspose.cells/protectedrange/isprotectedwithpassword/
---
## ProtectedRange.IsProtectedWithPassword property

يشير إلى ما إذا كانت أوراق العمل محمية بكلمة مرور.

```csharp
public bool IsProtectedWithPassword { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاقات محمية والحصول على مؤشراتها
            int protectedIndex = worksheet.AllowEditRanges.Add("PasswordProtected", 0, 0, 5, 5);
            ProtectedRange protectedWithPassword = worksheet.AllowEditRanges[protectedIndex];
            protectedWithPassword.Password = "test123";
            
            int unprotectedIndex = worksheet.AllowEditRanges.Add("Unprotected", 6, 0, 11, 5);
            ProtectedRange unprotected = worksheet.AllowEditRanges[unprotectedIndex];
            
            // حماية ورقة العمل لفرض القيود
            worksheet.Protect(ProtectionType.All);
            
            // التحقق من حالة حماية كلمة المرور
            Console.WriteLine($"Range '{protectedWithPassword.Name}' password protected: {protectedWithPassword.IsProtectedWithPassword}");
            Console.WriteLine($"Range '{unprotected.Name}' password protected: {unprotected.IsProtectedWithPassword}");
        }
    }
}
```

### انظر أيضًا

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


