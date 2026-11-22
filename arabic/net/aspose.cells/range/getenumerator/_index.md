---
title: "Range.GetEnumerator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. يحصل على المُعدِّد للخلية في هذا النطاق"
type: docs
url: /ar/net/aspose.cells/range/getenumerator/
---
## Range.GetEnumerator method

يحصل على المُعدِّد للخلية في هذا Range.

```csharp
public IEnumerator GetEnumerator()
```

### قيمة الإرجاع

The cells enumerator

### ملاحظات

عند استعراض العناصر باستخدام الـ Enumerator المعاد، يجب عدم تعديل مجموعة الخلايا (مثل العمليات التي قد تؤدي إلى إنشاء خلية/صف جديد أو حذف خلية/صف موجود). وإلا قد لا يتمكن الـ Enumerator من استعراض جميع الخلايا بشكل صحيح (قد يتم استعراض بعض العناصر عدة مرات أو يتم تخطيها).

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ بعض بيانات العينة
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["C2"].PutValue("Cherry");
            worksheet.Cells["C3"].PutValue("Date");

            // احصل على النطاق وعدّد الخلايا
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C3");
            IEnumerator enumerator = range.GetEnumerator();
            
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine($"{cell.Name}: {cell.Value}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


