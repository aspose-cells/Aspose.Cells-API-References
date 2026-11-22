---
title: "ProtectedRange.CellArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ProtectedRange. يحصل على كائن CellArea الذي يمثل منطقة الخلايا التي سيتم حمايتها"
type: docs
url: /ar/net/aspose.cells/protectedrange/cellarea/
---
## ProtectedRange.CellArea property

يحصل على كائن `CellArea` الذي يمثل منطقة الخلايا التي سيتم حمايتها.

```csharp
public CellArea CellArea { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاقات محمية
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
            
            // إضافة النطاق المحمي الأول
            int index1 = allowRanges.Add("Range1", 0, 0, 2, 2);
            ProtectedRange range1 = allowRanges[index1];
            range1.Password = "123";

            // إضافة النطاق المحمي الثاني
            int index2 = allowRanges.Add("Range2", 3, 3, 5, 5);
            ProtectedRange range2 = allowRanges[index2];
            range2.Password = "456";

            // عرض معلومات CellArea لكلا النطاقين
            Console.WriteLine("Protected Range 1:");
            Console.WriteLine($"Name: {range1.Name}");
            Console.WriteLine($"Area: {range1.CellArea.StartRow},{range1.CellArea.StartColumn} to {range1.CellArea.EndRow},{range1.CellArea.EndColumn}");

            Console.WriteLine("\nProtected Range 2:");
            Console.WriteLine($"Name: {range2.Name}");
            Console.WriteLine($"Area: {range2.CellArea.StartRow},{range2.CellArea.StartColumn} to {range2.CellArea.EndRow},{range2.CellArea.EndColumn}");

            // احفظ المصنف
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


