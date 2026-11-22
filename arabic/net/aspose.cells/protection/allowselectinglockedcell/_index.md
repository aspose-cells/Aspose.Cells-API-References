---
title: "Protection.AllowSelectingLockedCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان يُسمح للمستخدم باختيار الخلايا المقفلة في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/allowselectinglockedcell/
---
## Protection.AllowSelectingLockedCell property

يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا المقفلة في ورقة عمل محمية.

```csharp
public bool AllowSelectingLockedCell { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingLockedCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ضبط إعدادات الحماية
            Protection protection = worksheet.Protection;
            
            // عرض خاصية AllowSelectingLockedCell
            protection.AllowSelectingLockedCell = true;
            Console.WriteLine("AllowSelectingLockedCell is set to: " + protection.AllowSelectingLockedCell);

            // تعديل الخاصية وإظهار التغيير
            protection.AllowSelectingLockedCell = false;
            Console.WriteLine("AllowSelectingLockedCell is now set to: " + protection.AllowSelectingLockedCell);

            // حماية ورقة العمل باستخدام كلمة مرور
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // احفظ المصنف
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


