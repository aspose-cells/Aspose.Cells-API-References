---
title: "AbstractLowCodeProtectionProvider.GetOpenPassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractLowCodeProtectionProvider. تحصل على كلمة المرور لفتح ملف جدول البيانات"
type: docs
url: /ar/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/
---
## AbstractLowCodeProtectionProvider.GetOpenPassword method

يحصل على كلمة المرور لفتح ملف الجدول.

```csharp
public virtual string GetOpenPassword()
```

### قيمة الإرجاع

كلمة المرور لفتح ملف جدول البيانات. فارغ يعني عدم وجود حماية لفتح الملف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مثيل لمزود الحماية
                var protectionProvider = new DemoProtectionProvider();

                // استدعاء طريقة GetOpenPassword لاسترجاع كلمة المرور
                string password = protectionProvider.GetOpenPassword();

                // إنشاء دفتر عمل جديد وتطبيق كلمة المرور
                Workbook workbook = new Workbook("sample.xlsx");
                workbook.Settings.Password = password;

                // حفظ دفتر العمل المحمي بكلمة مرور
                workbook.Save("MethodGetOpenPasswordDemo.xlsx");

                Console.WriteLine($"Workbook protected with open password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword()
        {
            return "AsposeDemo123!";
        }
    }
}
```

### انظر أيضًا

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


