---
title: "UnionRange.ColumnCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnionRange. تحصل على عدد الصفوف في النطاق"
type: docs
url: /ar/net/aspose.cells/unionrange/columncount/
---
## UnionRange.ColumnCount property

يحصل على عدد الصفوف في النطاق.

```csharp
public int ColumnCount { get; }
```

### ملاحظات

يؤثر فقط عندما يحتوي على نطاق واحد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = 1200;
            worksheet.Cells["C2"].Value = 5;
            worksheet.Cells["A3"].Value = "Phone";
            worksheet.Cells["B3"].Value = 800;
            worksheet.Cells["C3"].Value = 10;

            try
            {
                // إنشاء نطاقات ودمجها في نطاق اتحاد
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C2");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A3:C3");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // اعرض قيمة خاصية ColumnCount
                Console.WriteLine("ColumnCount of union range: " + unionRange.ColumnCount);

                // أظهر الاستخدام من خلال عرض معلومات الأعمدة
                Console.WriteLine("First column index: " + unionRange.FirstColumn);
                Console.WriteLine("Last column index: " + (unionRange.FirstColumn + unionRange.ColumnCount - 1));

                // أنشئ نطاق اتحاد آخر بعدد أعمدة مختلف
                Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A1:B2");
                Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("D1:E2");
                UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

                // قارن عدد الأعمدة
                Console.WriteLine("Second union range ColumnCount: " + unionRange2.ColumnCount);
                Console.WriteLine("First union range has " +
                    (unionRange.ColumnCount > unionRange2.ColumnCount ? "more" : "fewer") +
                    " columns than second union range");

                // احفظ المصنف
                workbook.Save("UnionRangeColumnCountDemo.xlsx");
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


