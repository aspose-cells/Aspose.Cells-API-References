---
title: "FilterColumn.Top10Filter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. تحصل على Top10Filter لتصفية البيانات حسب ترتيب البيانات"
type: docs
url: /ar/net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

تحصل على `Top10Filter` لتصفية البيانات حسب ترتيب البيانات.

```csharp
public Top10Filter Top10Filter { get; }
```

### ملاحظات

قبل استخدام هذه الخاصية، يرجى التأكد من أن [`FilterType`](../filtertype/) هو Top10، وإلا سيتم إرجاع null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // املأ بعض بيانات العينة
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // طبق AutoFilter على نطاق البيانات
                sheet.AutoFilter.Range = "A1:A5";

                // احصل على عمود الفلتر الأول (فهرس العمود 0)
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // اعرض كائن Filter الحالي (قد يكون null)
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // تحقق مما إذا كان الفلتر المطبق هو Top10Filter
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // احفظ دفتر العمل (اختياري)
                workbook.Save("Top10FilterDemo.xlsx");
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

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


