---
title: "FindOptions.IsRangeSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. تشير إلى ما إذا كان النطاق الذي تم البحث فيه محددًا"
type: docs
url: /ar/net/aspose.cells/findoptions/israngeset/
---
## FindOptions.IsRangeSet property

يشير إلى ما إذا كان النطاق الذي تم البحث فيه محددًا.

```csharp
public bool IsRangeSet { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertyIsRangeSetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Date");
            worksheet.Cells["B2"].PutValue("Elderberry");
            worksheet.Cells["B3"].PutValue("Fig");

            // أنشئ مثيل FindOptions
            FindOptions findOptions = new FindOptions();

            // تحقق من القيمة الأولية لـ IsRangeSet (يجب أن تكون false)
            Console.WriteLine("Initial IsRangeSet value: " + findOptions.IsRangeSet);

            // حدد نطاق بحث
            CellArea searchRange = new CellArea();
            searchRange.StartRow = 0;
            searchRange.StartColumn = 0;
            searchRange.EndRow = 2;
            searchRange.EndColumn = 0; // Column A only
            findOptions.SetRange(searchRange);

            // تحقق من IsRangeSet بعد تحديد النطاق (يجب أن تكون true)
            Console.WriteLine("After SetRange, IsRangeSet value: " + findOptions.IsRangeSet);

            // نفّذ عملية بحث داخل النطاق المحدد
            Cell foundCell = worksheet.Cells.Find("Banana", null, findOptions);
            Console.WriteLine("Found 'Banana' at: " + foundCell?.Name);

            // حاول العثور على شيء خارج النطاق (يجب ألا يُعثر عليه)
            foundCell = worksheet.Cells.Find("Fig", null, findOptions);
            Console.WriteLine("Found 'Fig' at: " + foundCell?.Name); // Should be null

            // احفظ المصنف
            workbook.Save("PropertyIsRangeSetDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


