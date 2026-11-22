---
title: "VbaProject.ValidatePassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaProject. تتحقق من صحة كلمة مرور الحماية"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/validatepassword/
---
## VbaProject.ValidatePassword method

يتحقق من صحة كلمة مرور الحماية.

```csharp
public bool ValidatePassword(string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| كلمة المرور | String | كلمة المرور |

### قيمة الإرجاع

ما إذا كانت كلمة المرور هي كلمة مرور الحماية لهذا مشروع VBA

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل من ملف Excel نموذجي يحتوي على مشروع VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // تحقق من صحة كلمة مرور مشروع VBA
            bool isValid = workbook.VbaProject.ValidatePassword("test");
            
            // إخراج نتيجة التحقق
            Console.WriteLine("Password validation result: " + isValid);
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


