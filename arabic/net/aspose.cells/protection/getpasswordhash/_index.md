---
title: "Protection.GetPasswordHash"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Protection. تحصل على التجزئة لكلمة المرور الحالية"
type: docs
url: /ar/net/aspose.cells/protection/getpasswordhash/
---
## Protection.GetPasswordHash method

يحصل على تجزئة كلمة المرور الحالية.

```csharp
public int GetPasswordHash()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodGetPasswordHashDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // عيّن إعدادات الحماية باستخدام كلمة المرور
            Protection protection = worksheet.Protection;
            protection.Password = "password123";
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingCell = true;
            
            // حماية ورقة العمل
            worksheet.Protect(ProtectionType.All);

            try
            {
                // احصل على تجزئة كلمة المرور
                int passwordHash = protection.GetPasswordHash();
                
                // اعرض النتيجة
                Console.WriteLine($"Password hash: {passwordHash}");
                Console.WriteLine($"Is protected with password: {protection.IsProtectedWithPassword}");

                // تحقق من كلمة المرور (لتوضيح الوظيفة ذات الصلة)
                bool isVerified = protection.VerifyPassword("password123");
                Console.WriteLine($"Password verification result: {isVerified}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPasswordHash method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("ProtectionMethodGetPasswordHashDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


