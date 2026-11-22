---
title: "WriteProtection.Password"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WriteProtection. تعيين كلمة المرور المحمية لتعديل الملف"
type: docs
url: /ar/net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

يضبط كلمة المرور المحمية لتعديل الملف.

```csharp
public string Password { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن كلمة مرور حماية الكتابة
            workbook.Settings.WriteProtection.Password = "owner";
            
            // احفظ المصنف
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            Console.WriteLine("Workbook write-protected with password successfully.");
        }
    }
}
```

### انظر أيضًا

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


