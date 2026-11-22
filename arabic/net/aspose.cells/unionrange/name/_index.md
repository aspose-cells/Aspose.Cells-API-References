---
title: "UnionRange.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnionRange. تحصل أو تعين اسم النطاق"
type: docs
url: /ar/net/aspose.cells/unionrange/name/
---
## UnionRange.Name property

يحصل أو يضبط اسم النطاق.

```csharp
public string Name { get; set; }
```

### ملاحظات

النطاق المسمى مدعوم. على سبيل المثال،

range.Name = "Sheet1!MyRange";

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].Value = "First Range";
            worksheet.Cells["B2"].Value = "Second Range";

            try
            {
                // إنشاء نطاقات ودمجها في نطاق اتحاد
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:A1");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:B2");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // اعرض القيمة الحالية لخاصية Name
                Console.WriteLine("Initial Name value: " + unionRange.Name);

                // عيّن اسمًا جديدًا لنطاق الاتحاد
                unionRange.Name = "MyUnionRange";
                Console.WriteLine("Updated Name value: " + unionRange.Name);

                // أظهر أن الاسم يمكن تغييره مرة أخرى
                unionRange.Name = "CustomUnionRange";
                Console.WriteLine("Final Name value: " + unionRange.Name);

                // احفظ المصنف
                workbook.Save("UnionRangeNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


