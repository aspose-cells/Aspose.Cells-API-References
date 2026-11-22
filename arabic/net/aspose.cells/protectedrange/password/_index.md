---
title: "ProtectedRange.Password"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ProtectedRange. تمثل كلمة المرور لحماية النطاق"
type: docs
url: /ar/net/aspose.cells/protectedrange/password/
---
## ProtectedRange.Password property

يمثل كلمة المرور لحماية النطاق.

```csharp
public string Password { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyPasswordDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة نطاقات محمية
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // إضافة نطاق محمي
            int index = allowRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];

            // تعيين كلمة مرور للنطاق المحمي
            protectedRange.Password = "12345";

            // احفظ المصنف
            workbook.Save("ProtectedRangeWithPassword.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


