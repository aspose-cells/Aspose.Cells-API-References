---
title: "AbstractLowCodeProtectionProvider.GetWritePassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractLowCodeProtectionProvider. تحصل على كلمة المرور لتعديل ملف الجدول"
type: docs
url: /ar/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/
---
## AbstractLowCodeProtectionProvider.GetWritePassword method

يحصل على كلمة المرور لتعديل ملف الجدول.

```csharp
public virtual string GetWritePassword()
```

### قيمة الإرجاع

كلمة المرور لتعديل ملف الجدول. فارغ يعني عدم وجود حماية لتعديل الملف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWritePasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // إنشاء مثال لمزود الحماية المخصص
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                // استدعاء GetWritePassword صراحةً وعرض النتيجة
                string writePassword = protectionProvider.GetWritePassword();
                Console.WriteLine($"Retrieved write password: {writePassword}");

                // حفظ دفتر العمل - تطبيق حماية الكتابة مباشرة
                workbook.Settings.WriteProtection.Password = writePassword;
                workbook.Save("MethodGetWritePasswordDemo.xlsx");
                Console.WriteLine("Workbook saved with write protection password.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWritePassword method: {ex.Message}");
            }
        }

    }

    // تنفيذ مخصص لمزود الحماية
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWritePassword()
        {
            return "AsposeTestPassword123!";
        }

        // تنفيذ الطرق المطلوبة الأخرى مع القيم الافتراضية
        public override string GetOpenPassword() => null;
        public override string GetWorkbookPassword() => null;
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### انظر أيضًا

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


