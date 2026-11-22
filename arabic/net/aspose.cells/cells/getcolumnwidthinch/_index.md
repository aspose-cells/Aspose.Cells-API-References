---
title: "Cells.GetColumnWidthInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على عرض العمود المحدد في العرض العادي بوحدات البوصة"
type: docs
url: /ar/net/aspose.cells/cells/getcolumnwidthinch/
---
## Cells.GetColumnWidthInch method

يحصل على عرض العمود المحدد في العرض العادي، بوحدات البوصة.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnWidthInch(int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود |

### قيمة الإرجاع

عرض العمود

عرض العمود في العرض العادي.

### ملاحظات

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Cells.GetColumnWidth(int ,bool , CellsUnitType ). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthInchWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين عرض العمود بالبوصة للتوضيح
            int columnIndex = 2;
            cells.SetColumnWidthInch(columnIndex, 2.5);

            try
            {
                // استدعاء GetColumnWidthInch مع معلمة Int32
                double columnWidth = cells.GetColumnWidthInch(columnIndex);

                // عرض النتيجة
                Console.WriteLine($"Width of column {columnIndex} in inches: {columnWidth}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthInch method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("CellsMethodGetColumnWidthInchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


