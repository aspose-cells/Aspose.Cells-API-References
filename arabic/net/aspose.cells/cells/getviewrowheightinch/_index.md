---
title: "Cells.GetViewRowHeightInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على ارتفاع صف محدد بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/cells/getviewrowheightinch/
---
## Cells.GetViewRowHeightInch method

يحصل على ارتفاع صف محدد بوحدة البوصة.

```csharp
public double GetViewRowHeightInch(int row)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف |

### قيمة الإرجاع

ارتفاع الصف

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetViewRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين ارتفاع صف مخصص للصف 2 بالبوصة
            worksheet.Cells.SetRowHeightInch(2, 1.5);

            try
            {
                // استدعاء GetViewRowHeightInch مع معامل فهرس الصف
                double rowHeight = worksheet.Cells.GetViewRowHeightInch(2);
                
                // عرض النتيجة والتحقق من أن الارتفاع يطابق القيمة المحددة
                Console.WriteLine($"View row height of row 2: {rowHeight} inches");
                
                // إظهار التأثير بإضافة محتوى تجريبي
                worksheet.Cells["A2"].PutValue($"Row Height: {rowHeight}\"");
                worksheet.Cells.SetColumnWidthInch(0, 15);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetViewRowHeightInch: {ex.Message}");
            }
            
            // احفظ المصنف المعدل
            workbook.Save("CellsMethodGetViewRowHeightInchWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


