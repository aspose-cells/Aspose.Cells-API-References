---
title: "WriteProtection.ValidatePassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WriteProtection. تُعيد true إذا كانت كلمة المرور المحددة هي نفسها كلمة مرور الحماية التي تم حماية الملف بها"
type: docs
url: /ar/net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

يرجع true إذا كانت كلمة المرور المحددة هي نفسها كلمة مرور الحماية للكتابة التي تم حماية الملف بها.

```csharp
public bool ValidatePassword(string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| كلمة المرور | String | كلمة المرور المحددة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // عيّن كلمة مرور حماية الكتابة
            workbook.Settings.WriteProtection.Password = "1234";
            
            // تحقق من كلمة المرور
            Console.WriteLine("Password '1234' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            Console.WriteLine("Password 'wrong' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("wrong"));
        }
    }
}
```

### انظر أيضًا

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


