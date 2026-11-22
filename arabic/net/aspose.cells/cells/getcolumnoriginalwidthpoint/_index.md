---
title: "Cells.GetColumnOriginalWidthPoint"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على ارتفاع العمود الأصلي بوحدة النقطة إذا كان العمود مخفيًا"
type: docs
url: /ar/net/aspose.cells/cells/getcolumnoriginalwidthpoint/
---
## Cells.GetColumnOriginalWidthPoint method

تحصل على ارتفاع العمود الأصلي بوحدة النقطة إذا كان العمود مخفيًا

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس الصف. |

### قيمة الإرجاع

عرض العمود في العرض العادي.

### ملاحظات

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Cells.GetColumnWidth(int ,bool , CellsUnitType ). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تحضير معامل فهرس العمود
            int columnIndex = 0;

            try
            {
                // احصل على عرض العمود الأصلي بالنقاط
                double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");

                // تعديل عرض العمود
                cells.SetColumnWidth(columnIndex, 15);
                Console.WriteLine("Set new column width to 15 points");

                // احصل على العرض الأصلي مرة أخرى لتوضيح أنه يبقى دون تغيير
                double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width remains: {unchangedWidth} points");

                // احصل على العرض الحالي لإظهار التعديل
                double currentWidth = cells.GetColumnWidth(columnIndex);
                Console.WriteLine($"Current column width: {currentWidth} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


