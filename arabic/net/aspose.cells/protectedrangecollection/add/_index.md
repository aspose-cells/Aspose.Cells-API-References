---
title: "ProtectedRangeCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ProtectedRangeCollection. تُضيف عنصر ProtectedRange إلى المجموعة"
type: docs
url: /ar/net/aspose.cells/protectedrangecollection/add/
---
## ProtectedRangeCollection.Add method

تضيف عنصر [`ProtectedRange`](../../protectedrange/) إلى المجموعة.

```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | عنوان النطاق. يُستخدم كواصف، وليس كتعريف نطاق مسمى. |
| startRow | Int32 | فهرس الصف الابتدائي للنطاق. |
| startColumn | Int32 | فهرس العمود الابتدائي للنطاق. |
| endRow | Int32 | فهرس الصف النهائي للنطاق. |
| endColumn | Int32 | فهرس العمود النهائي للنطاق. |

### قيمة الإرجاع

فهرس الكائن.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionMethodAddWithStringInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
            
            // إضافة نطاق محمي بالاسم والإحداثيات
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            
            // الوصول إلى النطاق المضاف
            ProtectedRange range = pranges[index];
            
            // تعيين محدد الأمان
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            range.SecurityDescriptor = securityDescriptor;
            
            // حفظ والتحقق
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


