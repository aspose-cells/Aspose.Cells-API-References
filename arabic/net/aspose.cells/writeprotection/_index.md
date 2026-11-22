---
title: "الفئة WriteProtection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.WriteProtection. تحدد إعدادات الحماية للكتابة لدفتر العمل"
type: docs
url: /ar/net/aspose.cells/writeprotection/
---
## WriteProtection class

يحدد إعدادات الحماية من الكتابة للمصنف.

```csharp
public class WriteProtection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Author](../../aspose.cells/writeprotection/author/) { get; set; } | يحصل على المؤلف ويضبطه. |
| [IsWriteProtected](../../aspose.cells/writeprotection/iswriteprotected/) { get; } | يشير إلى ما إذا كان دفتر العمل محميًا للكتابة. |
| [Password](../../aspose.cells/writeprotection/password/) { get; set; } | يضبط كلمة المرور المحمية لتعديل الملف. |
| [RecommendReadOnly](../../aspose.cells/writeprotection/recommendreadonly/) { get; set; } | يشير إلى ما إذا تم اختيار خيار القراءة فقط الموصى به. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ValidatePassword](../../aspose.cells/writeprotection/validatepassword/)(string) | يرجع true إذا كانت كلمة المرور المحددة هي نفسها كلمة مرور الحماية للكتابة التي تم حماية الملف بها. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WriteProtectionDemo
    {
        public static void WriteProtectionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات دفتر العمل
            WorkbookSettings settings = workbook.Settings;

            // الوصول إلى إعدادات الحماية للكتابة
            WriteProtection writeProtection = settings.WriteProtection;

            // تعيين مؤلف الحماية من الكتابة
            writeProtection.Author = "John Doe";

            // تعيين كلمة المرور للحماية من الكتابة
            writeProtection.Password = "password123";

            // تعيين خيار القراءة فقط الموصى به
            writeProtection.RecommendReadOnly = true;

            // تحقق مما إذا كان المصنف محميًا من الكتابة
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine("Is Write Protected: " + isWriteProtected);

            // تحقق من صحة كلمة المرور
            bool isValidPassword = writeProtection.ValidatePassword("password123");
            Console.WriteLine("Is Valid Password: " + isValidPassword);

            // احفظ المصنف
            workbook.Save("WriteProtectionExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


