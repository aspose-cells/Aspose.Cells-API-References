---
title: "Protection.Password"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل كلمة المرور لحماية ورقة العمل"
type: docs
url: /ar/net/aspose.cells/protection/password/
---
## Protection.Password property

يمثل كلمة المرور لحماية ورقة العمل.

```csharp
public string Password { get; set; }
```

### ملاحظات

إذا تم تعيين كلمة المرور إلى null أو سلسلة فارغة، يمكنك إلغاء حماية ورقة العمل أو المصنف دون استخدام كلمة مرور. وإلا، يجب عليك تحديد كلمة المرور لإلغاء حماية ورقة العمل أو المصنف.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // عيّن إعدادات الحماية باستخدام كلمة المرور
            Protection protection = worksheet.Protection;
            protection.AllowEditingContent = false;
            protection.AllowDeletingColumn = false;
            protection.Password = "test123";

            // تحقق من حماية كلمة المرور
            Console.WriteLine("Worksheet is protected: " + (protection.Password != null));
            Console.WriteLine("Protection password: " + protection.Password);

            // أنشئ كائن حماية آخر للمقارنة
            Protection protection2 = worksheet.Protection;
            protection2.Password = "test123";

            // قارن حماية كلمة المرور
            Console.WriteLine("Passwords match: " + (protection.Password == protection2.Password));
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


