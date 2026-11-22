---
title: "ProtectedRange.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ProtectedRange. يحصل على عنوان النطاق. يُستخدم هذا كواصف وليس كتعريف نطاق مسمى"
type: docs
url: /ar/net/aspose.cells/protectedrange/name/
---
## ProtectedRange.Name property

يحصل على عنوان النطاق. يُستخدم هذا كواصف، وليس كتعريف نطاق مسمى.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة نطاقات محمية
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // إضافة نطاق محمي بالاسم "MyRange"
            int index = allowRanges.Add("MyRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];
            protectedRange.Password = "123";

            // الوصول إلى خاصية Name وعرضها
            Console.WriteLine("Protected range name: " + protectedRange.Name);
            Console.WriteLine("Cell area: {0},{1} to {2},{3}", 
                protectedRange.CellArea.StartRow,
                protectedRange.CellArea.StartColumn,
                protectedRange.CellArea.EndRow,
                protectedRange.CellArea.EndColumn);

            // إضافة نطاق مسمى آخر
            index = allowRanges.Add("SecondRange", 3, 3, 5, 5);
            ProtectedRange secondRange = allowRanges[index];
            Console.WriteLine("Second protected range name: " + secondRange.Name);

            // احفظ المصنف
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


