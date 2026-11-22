---
title: "Name.GetRanges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Name. تحصل على جميع النطاقات المشار إليها بهذا الاسم"
type: docs
url: /ar/net/aspose.cells/name/getranges/
---
## GetRanges() {#getranges}

يحصل على جميع النطاقات التي يُشير إليها هذا الاسم.

```csharp
public Range[] GetRanges()
```

### قيمة الإرجاع

جميع النطاقات.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            
            // إنشاء نطاق مسمى
            int index = workbook.Worksheets.Names.Add("Fruits");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // احصل على النطاقات مع إعادة الحساب
            Aspose.Cells.Range[] ranges1 = name.GetRanges();
            Console.WriteLine("Ranges with recalculation:");
            PrintRanges(ranges1);
            
            // احصل على النطاقات بدون إعادة الحساب
            Aspose.Cells.Range[] ranges2 = name.GetRanges(false);
            Console.WriteLine("\nRanges without recalculation:");
            PrintRanges(ranges2);
        }
        
        private static void PrintRanges(Aspose.Cells.Range[] ranges)
        {
            if (ranges != null)
            {
                foreach (Aspose.Cells.Range range in ranges)
                {
                    Console.WriteLine($"Range: {range.Address}");
                }
            }
            else
            {
                Console.WriteLine("No ranges found");
            }
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRanges(bool) {#getranges_1}

يحصل على جميع النطاقات التي يُشير إليها هذا الاسم.

```csharp
public Range[] GetRanges(bool recalculate)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| إعادة حساب | منطقي | ما إذا كان يجب إعادة حسابه إذا تم حساب هذا الاسم مسبقًا قبل هذا الاستدعاء. |

### قيمة الإرجاع

جميع النطاقات.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // إنشاء نطاق مسمى
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // احصل على النطاقات بدون إعادة حساب
            Aspose.Cells.Range[] ranges1 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count (no recalc): " + ranges1.Length);
            
            // احصل على النطاقات مع إعادة الحساب
            Aspose.Cells.Range[] ranges2 = namedRange.GetRanges();
            Console.WriteLine("Ranges count (with recalc): " + ranges2.Length);
            
            // عدّل النطاق وأظهر إعادة الحساب
            worksheet.Cells["A4"].PutValue(30);
            namedRange.RefersTo = "=Sheet1!$A$1:$A$4";
            
            // احصل على النطاقات مع وبدون إعادة الحساب بعد التعديل
            Aspose.Cells.Range[] ranges3 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count after mod (no recalc): " + ranges3.Length);
            
            Aspose.Cells.Range[] ranges4 = namedRange.GetRanges();
            Console.WriteLine("Ranges count after mod (with recalc): " + ranges4.Length);
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


