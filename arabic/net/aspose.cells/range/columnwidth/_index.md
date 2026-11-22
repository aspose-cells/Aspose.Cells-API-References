---
title: "Range.ColumnWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحدد أو يحصل على عرض العمود لهذا النطاق"
type: docs
url: /ar/net/aspose.cells/range/columnwidth/
---
## Range.ColumnWidth property

يضبط أو يحصل على عرض العمود لهذا النطاق

```csharp
public double ColumnWidth { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyColumnWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى نطاق (الأعمدة B إلى D)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B:D");
            
            // عرض عرض العمود الحالي
            Console.WriteLine("Current ColumnWidth: " + range.ColumnWidth);

            // تعيين عرض عمود جديد (بوحدات الأحرف)
            range.ColumnWidth = 15.0;

            // ملء الخلايا لإظهار التأثير
            worksheet.Cells["B1"].PutValue("This is column B");
            worksheet.Cells["C1"].PutValue("This is column C");
            worksheet.Cells["D1"].PutValue("This is column D");

            // ضبط تلقائي للصفوف لعرض المحتوى
            worksheet.AutoFitRows();

            // احفظ المصنف
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


