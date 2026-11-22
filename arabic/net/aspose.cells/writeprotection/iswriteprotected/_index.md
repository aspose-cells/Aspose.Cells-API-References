---
title: "WriteProtection.IsWriteProtected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WriteProtection. تشير إلى ما إذا كان هذا المصنف محميًا من الكتابة"
type: docs
url: /ar/net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

يشير إلى ما إذا كان دفتر العمل محميًا للكتابة.

```csharp
public bool IsWriteProtected { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyIsWriteProtectedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // فعّل حماية الكتابة باستخدام كلمة مرور
            workbook.Settings.WriteProtection.Password = "1234";
            
            // تحقق مما إذا كان المصنف محميًا من الكتابة
            Console.WriteLine("Is workbook write protected? " + 
                workbook.Settings.WriteProtection.IsWriteProtected);
            
            // تحقق من صحة كلمة المرور
            Console.WriteLine("Is password valid? " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            
            // احفظ المصنف
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            // حمّل المصنف المحفوظ للتحقق من الحماية
            Workbook loadedWorkbook = new Workbook("WriteProtectedWorkbook.xlsx");
            
            // تحقق من حالة الحماية مرة أخرى
            Console.WriteLine("Is loaded workbook write protected? " + 
                loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### انظر أيضًا

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


