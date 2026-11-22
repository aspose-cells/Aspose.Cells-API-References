---
title: "Protection.IsProtectedWithPassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تشير إلى ما إذا كانت ورقة العمل محمية بكلمة مرور"
type: docs
url: /ar/net/aspose.cells/protection/isprotectedwithpassword/
---
## Protection.IsProtectedWithPassword property

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
    public class ProtectionPropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى إعدادات حماية ورقة العمل
            Protection protection = worksheet.Protection;

            // عيّن كلمة مرور الحماية
            protection.Password = "test123";

            // تحقق مما إذا كانت ورقة العمل محمية بكلمة مرور
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;
            Console.WriteLine("Is worksheet protected with password: " + isProtectedWithPassword);

            // احفظ المصنف
            workbook.Save("PasswordProtectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


