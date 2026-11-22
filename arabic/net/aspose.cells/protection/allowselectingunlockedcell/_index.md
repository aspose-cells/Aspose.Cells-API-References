---
title: "Protection.AllowSelectingUnlockedCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا غير المؤمنة في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/allowselectingunlockedcell/
---
## Protection.AllowSelectingUnlockedCell property

يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا غير المقفلة في ورقة عمل محمية.

```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingUnlockedCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // حماية ورقة العمل بجميع خيارات الحماية
            Protection protection = worksheet.Protection;
            
            // ضبط AllowSelectingUnlockedCell إلى true
            protection.AllowSelectingUnlockedCell = true;
            protection.AllowSelectingLockedCell = false;
            
            // تطبيق الحماية باستخدام كلمة مرور
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // تحقق من الإعداد
            Console.WriteLine("AllowSelectingUnlockedCell: " + protection.AllowSelectingUnlockedCell);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);

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


