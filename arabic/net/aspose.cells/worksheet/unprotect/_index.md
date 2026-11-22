---
title: "Worksheet.Unprotect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Worksheet method. يزيل حماية ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/unprotect/
---
## Unprotect() {#unprotect}

يفك حماية ورقة العمل.

```csharp
public void Unprotect()
```

### ملاحظات

هذه الطريقة تزيل حماية ورقة العمل التي تم حمايتها بدون كلمة مرور.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodUnprotectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احمِ ورقة العمل باستخدام كلمة مرور
            worksheet.Protect(ProtectionType.All, "password123", null);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
            
            try
            {
                // أزل حماية ورقة العمل بدون كلمة مرور (يجب أن يفشل)
                worksheet.Unprotect();
                Console.WriteLine("Worksheet unprotected without password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect without password: " + ex.Message);
            }

            try
            {
                // أزل حماية ورقة العمل باستخدام كلمة مرور خاطئة (يجب أن يفشل)
                worksheet.Unprotect("wrongpassword");
                Console.WriteLine("Worksheet unprotected with wrong password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect with wrong password: " + ex.Message);
            }

            try
            {
                // إلغاء حماية ورقة العمل باستخدام كلمة المرور الصحيحة
                worksheet.Unprotect("password123");
                Console.WriteLine("Worksheet successfully unprotected: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect: " + ex.Message);
            }
            
            // حفظ النتيجة
            workbook.Save("WorksheetMethodUnprotectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Unprotect(string) {#unprotect_1}

يفك حماية ورقة العمل.

```csharp
public void Unprotect(string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| كلمة المرور | String | كلمة المرور |

### ملاحظات

إذا كانت ورقة العمل محمية بدون كلمة مرور، يمكنك تعيين قيمة فارغة أو سلسلة فارغة إلى معلمة كلمة المرور.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // حماية ورقة العمل باستخدام كلمة مرور ونوع الحماية الافتراضي
            worksheet.Protect(ProtectionType.All, "test", null);
            
            // إلغاء حماية ورقة العمل باستخدام كلمة مرور
            worksheet.Unprotect("test");
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


