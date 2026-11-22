---
title: "Range.ClearComments"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تمسح تعليقات هذا النطاق"
type: docs
url: /ar/net/aspose.cells/range/clearcomments/
---
## Range.ClearComments method

يمسح تعليقات هذا النطاق.

```csharp
public void ClearComments()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearCommentsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات والتعليقات إلى الخلايا
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A1"].PutValue("This is a comment on A1", true, false);
            worksheet.Cells["B2"].Value = "More Data";
            worksheet.Cells["B2"].PutValue("This is a comment on B2", true, false);

            try
            {
                // إنشاء نطاق يتضمن خلايا تحتوي على تعليقات
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // مسح التعليقات من النطاق
                range.ClearComments();

                Console.WriteLine("Comments cleared successfully from range A1:B2");
                Console.WriteLine($"Cell A1 value after clearing: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell B2 value after clearing: {worksheet.Cells["B2"].Value}");

                // احفظ المصنف
                workbook.Save("ClearCommentsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearComments: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


