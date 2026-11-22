---
title: "FindOptions.ConvertNumericData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم تحويل قيمة السلسلة التي تم البحث عنها إلى بيانات رقمية"
type: docs
url: /ar/net/aspose.cells/findoptions/convertnumericdata/
---
## FindOptions.ConvertNumericData property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يتم تحويل قيمة السلسلة التي تم البحث عنها إلى بيانات رقمية.

```csharp
public bool ConvertNumericData { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة تشمل القيم الرقمية كسلاسل نصية
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("456");
            worksheet.Cells["A3"].PutValue("01/28/2010");

            // أنشئ خيارات البحث واضبط ConvertNumericData إلى true
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;

            // ابحث عن قيمة التاريخ (مخزنة كسلسلة ولكن يتم تحويلها إلى رقمية أثناء البحث)
            Cell foundCell = worksheet.Cells.Find("01/28/2010", null, options);

            // أخرج النتيجة.
            if (foundCell != null)
            {
                Console.WriteLine("Found value at: " + foundCell.Name);
                Console.WriteLine("Cell value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("Value not found");
            }
        }
    }
}
```

### انظر أيضًا

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


