---
title: "تعداد EncryptionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.EncryptionType. نوع التشفير. يُستخدم فقط بواسطة excel2003. سنقوم بتشفير مصنف 2007/2010 باستخدام SHA AES كما يفعل Excel وسيتم تجاهل هذا EncryptionType"
type: docs
url: /ar/net/aspose.cells/encryptiontype/
---
## EncryptionType enumeration

نوع التشفير. يُستخدم فقط بواسطة excel2003. سنقوم بتشفير مصنف 2007/2010 باستخدام SHA AES كما تفعل Excel، وسيتم تجاهل EncryptionType هذا.

```csharp
public enum EncryptionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| XOR | `0` | خوارزمية تشفير XOR. |
| Compatible | `1` | متوافق مع Office 97/2000. |
| EnhancedCryptographicProviderV1 | `2` | تشفير محسّن. |
| StrongCryptographicProvider | `3` | خوارزمية تشفير قوية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EncryptionTypeDemo
    {
        public static void EncryptionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // تعيين خيارات التشفير للمصنف
            EncryptionType encryptionType = EncryptionType.EnhancedCryptographicProviderV1;
            int keyLength = 128; // Key length can be 40, 128, or 256 bits

            // تطبيق إعدادات التشفير
            workbook.SetEncryptionOptions(encryptionType, keyLength);

            // حماية المصنف باستخدام كلمة مرور
            string password = "securePassword";
            workbook.Protect(ProtectionType.All, password);

            // احفظ المصنف
            workbook.Save("EncryptedWorkbook.xlsx");
            workbook.Save("EncryptedWorkbook.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


