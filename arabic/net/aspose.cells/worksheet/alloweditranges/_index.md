---
title: "Worksheet.AllowEditRanges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على مجموعة نطاقات السماح بالتحرير في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

يحصل على مجموعة نطاقات السماح بالتعديل في ورقة العمل.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAllowEditRangesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة نطاق سماح بالتحرير
            int index = worksheet.AllowEditRanges.Add("r1", 0, 0, 1, 1);
            ProtectedRange range = worksheet.AllowEditRanges[index];
            range.Password = "password123";

            // حماية ورقة العمل
            worksheet.Protect(ProtectionType.All);

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // قم بتحميل المصنف المحفوظ للتحقق
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            ProtectedRange verifyRange = verifyWorkbook.Worksheets[0].AllowEditRanges[0];
            Console.WriteLine("Is protected with password: " + verifyRange.IsProtectedWithPassword);
        }
    }
}
```

### انظر أيضًا

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


