---
title: "AbstractLowCodeProtectionProvider.GetWorksheetPassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractLowCodeProtectionProvider. تحصل على كلمة المرور لحماية ورقة العمل المحددة"
type: docs
url: /ar/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/
---
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method

يحصل على كلمة المرور لحماية ورقة العمل المحددة.

```csharp
public virtual string GetWorksheetPassword(string sheetName)
```

### قيمة الإرجاع

كلمة المرور لحماية ورقة العمل المحددة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // إنشاء مثال لمزود الحماية المخصص
            var provider = new CustomProtectionProvider();

            try
            {
                // استدعاء GetWorksheetPassword مع اسم ورقة العمل
                string password = provider.GetWorksheetPassword(sheetName);

                // تطبيق الحماية على ورقة العمل باستخدام كلمة المرور المسترجعة
                worksheet.Protect(ProtectionType.All, password, null);

                Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
            }

            // حفظ دفتر العمل المحمي
            workbook.Save("WorksheetPasswordDemo.xlsx");

        }
    }

    // تنفيذ مخصص يُعيد كلمة المرور بناءً على اسم الورقة
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public new string GetWorksheetPassword(string sheetName)
        {
            // منطق بسيط لتوليد كلمة المرور لأغراض العرض
            return $"pw_{sheetName}";
        }
    }
}
```

### انظر أيضًا

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


