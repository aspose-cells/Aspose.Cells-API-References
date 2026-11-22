---
title: "ProtectedRangeCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ProtectedRangeCollection. تحصّل على عنصر ProtectedRange عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/protectedrangecollection/item/
---
## ProtectedRangeCollection indexer

تحصّل على عنصر [`ProtectedRange`](../../protectedrange/) عند الفهرس المحدد.

```csharp
public ProtectedRange this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة نطاق محمي باستخدام مؤشرات الخلايا (startRow, startColumn, endRow, endColumn)
            int index = worksheet.AllowEditRanges.Add("MyProtectedRange", 0, 0, 1, 1);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[index];
            protectedRange.Password = "password123";
            
            // الوصول إلى النطاق المحمي باستخدام خاصية Item (الفهرس 0)
            ProtectedRange retrievedRange = worksheet.AllowEditRanges[0];
            
            // التحقق وعرض حالة الحماية
            Console.WriteLine("Is protected with password: " + retrievedRange.IsProtectedWithPassword);
            Console.WriteLine("Range name: " + retrievedRange.Name);
            
            // احفظ المصنف
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


