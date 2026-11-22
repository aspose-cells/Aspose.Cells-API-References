---
title: "Cells.GetEnumerator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على مُعدِّد الخلايا"
type: docs
url: /ar/net/aspose.cells/cells/getenumerator/
---
## Cells.GetEnumerator method

يحصل على عداد الخلايا.

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
    public class CellsMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            
            // احصل على الـ Enumerator وتكرّر عبر الخلايا
            IEnumerator enumerator = worksheet.Cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                if (cell.Value != null)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


