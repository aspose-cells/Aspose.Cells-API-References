---
title: "ProtectedRange.GetAreas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ProtectedRange. يحصل على جميع المناطق المشار إليها"
type: docs
url: /ar/net/aspose.cells/protectedrange/getareas/
---
## ProtectedRange.GetAreas method

يحصل على جميع المساحات المُشار إليها.

```csharp
public CellArea[] GetAreas()
```

### قيمة الإرجاع

يعيد جميع المناطق المشار إليها.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeMethodGetAreasDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على مجموعة النطاقات المحمية
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // إضافة نطاق محمي
            int index = protectedRanges.Add("TestRange", 0, 0, 10, 10);
            ProtectedRange protectedRange = protectedRanges[index];
            
            // احصل على مناطق النطاق المحمي
            CellArea[] areas = protectedRange.GetAreas();
            
            // إخراج عدد المناطق (يجب أن يكون 1 لهذا النطاق البسيط)
            Console.WriteLine("Number of areas in protected range: " + areas.Length);
            
            // احفظ المصنف
            workbook.Save("ProtectedRangeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


