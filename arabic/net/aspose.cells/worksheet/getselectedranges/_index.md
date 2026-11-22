---
title: "Worksheet.GetSelectedRanges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحصل على النطاقات المحددة من الخلايا في جدول البيانات المصمم"
type: docs
url: /ar/net/aspose.cells/worksheet/getselectedranges/
---
## Worksheet.GetSelectedRanges method

يحصل على النطاقات المختارة من الخلايا في جدول البيانات المصمم.

```csharp
[Obsolete("Use Worksheet.GetSelectedAreas() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetSelectedRanges()
```

### قيمة الإرجاع

قائمة ArrayList تحتوي على النطاقات المحددة.

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Worksheet.GetSelectedAreas(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2025. تقدم Aspose اعتذارًا عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class WorksheetMethodGetSelectedRangesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "Test Value";

            try
            {
                // ملاحظة: تم وضع علامة GetSelectedRanges كمهجورة في الانعكاس
                // هذا يوضح استدعاء الطريقة كما هو مطلوب
                ArrayList selectedRanges = worksheet.GetSelectedRanges();

                // اعرض عدد النطاقات المحددة
                Console.WriteLine($"Number of selected ranges: {selectedRanges.Count}");

                // اعرض كل نطاق محدد
                foreach (var range in selectedRanges)
                {
                    Console.WriteLine($"Selected range: {range}");
                }

                // احفظ المصنف
                workbook.Save("GetSelectedRangesDemo.xlsx");
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

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


