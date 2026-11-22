---
title: "Protection.VerifyPassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Protection. تتحقق من كلمة المرور"
type: docs
url: /ar/net/aspose.cells/protection/verifypassword/
---
## Protection.VerifyPassword method

يتحقق من كلمة المرور.

```csharp
public bool VerifyPassword(string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| كلمة المرور | String | كلمة المرور. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodVerifyPasswordWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احمِ ورقة العمل باستخدام كلمة مرور
            worksheet.Protection.AllowDeletingColumn = false;
            worksheet.Protection.AllowDeletingRow = false;
            worksheet.Protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            try
            {
                // تحقق من كلمة المرور
                bool isPasswordCorrect = worksheet.Protection.VerifyPassword("password123");
                
                Console.WriteLine($"Password verification result: {isPasswordCorrect}");
                
                if (isPasswordCorrect)
                {
                    Console.WriteLine("The provided password matches the worksheet protection password.");
                }
                else
                {
                    Console.WriteLine("The provided password does not match the worksheet protection password.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing VerifyPassword method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("ProtectionMethodVerifyPasswordWithStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


