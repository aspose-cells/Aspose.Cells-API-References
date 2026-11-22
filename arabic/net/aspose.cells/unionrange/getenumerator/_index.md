---
title: "UnionRange.GetEnumerator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnionRange. تحصل على المُعدِّد للخلية في هذا النطاق"
type: docs
url: /ar/net/aspose.cells/unionrange/getenumerator/
---
## UnionRange.GetEnumerator method

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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class UnionRangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء النطاق الأول (A1:B2) وتعبئته بالبيانات
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1", "B2");
            range1[0, 0].PutValue("R1C1");
            range1[0, 1].PutValue("R1C2");
            range1[1, 0].PutValue("R2C1");
            range1[1, 1].PutValue("R2C2");

            // إنشاء النطاق الثاني (C1:D2) وتعبئته بالبيانات
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1", "D2");
            range2[0, 0].PutValue("R1C3");
            range2[0, 1].PutValue("R1C4");
            range2[1, 0].PutValue("R2C3");
            range2[1, 1].PutValue("R2C4");

            try
            {
                // بناء UnionRange من النطاق الأول
                UnionRange unionRange = worksheet.Cells
                    .CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { range1 });

                // إضافة النطاق الثاني إلى الاتحاد
                unionRange = unionRange.Union("C1:D2");

                // الحصول على المُعدِّد والتكرار عبر جميع الخلايا في الاتحاد
                IEnumerator enumerator = unionRange.GetEnumerator();
                Console.WriteLine("Enumerating cells in the UnionRange:");
                while (enumerator.MoveNext())
                {
                    Cell cell = enumerator.Current as Cell;
                    if (cell != null)
                    {
                        Console.WriteLine($"{cell.Name}: {cell.Value}");
                    }
                }

                // حفظ المصنف (اختياري، فقط لإظهار بقاء البيانات)
                workbook.Save("UnionRangeGetEnumeratorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetEnumerator: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


