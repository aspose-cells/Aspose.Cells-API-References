---
title: "FindOptions.SearchOrderByRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. تشير إلى ما إذا كان ترتيب البحث حسب الصفوف أو الأعمدة"
type: docs
url: /ar/net/aspose.cells/findoptions/searchorderbyrows/
---
## FindOptions.SearchOrderByRows property

يشير إلى ما إذا كان ترتيب البحث حسب الصفوف أو الأعمدة.

```csharp
public bool SearchOrderByRows { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchOrderByRowsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وإضافة بيانات نموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء الخلايا ببيانات اختبار (البحث عن "abc" بترتيب عمودي)
            worksheet.Cells["A1"].PutValue("xyz");
            worksheet.Cells["B1"].PutValue("def");
            worksheet.Cells["A2"].PutValue("123");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("abc");
            worksheet.Cells["B3"].PutValue("789");

            // إنشاء خيارات البحث وتعيين ترتيب البحث إلى عمودي
            FindOptions findOptions = new FindOptions();
            findOptions.SearchOrderByRows = false; // Search column by column

            // ابحث عن "abc" - يجب أن يُعيد A3 (الصف 2، العمود 0) عند البحث بترتيب عمودي
            Cell foundCell = worksheet.Cells.Find("abc", null, findOptions);

            // أخرج النتيجة.
            Console.WriteLine($"Found 'abc' at row: {foundCell.Row}, column: {foundCell.Column}");
        }
    }
}
```

### انظر أيضًا

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


