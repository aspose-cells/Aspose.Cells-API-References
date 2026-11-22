---
title: "Cells.GetColumnWidthPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. يحصل على عرض العمود المحدد في العرض العادي بوحدات البكسل"
type: docs
url: /ar/net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

يحصل على عرض العمود المحدد في العرض العادي، بوحدة البكسل.

```csharp
public int GetColumnWidthPixel(int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود |

### قيمة الإرجاع

عرض العمود في العرض العادي.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين عرض العمود بالأحرف (سيتم تحويله إلى بكسلات)
            worksheet.Cells.SetColumnWidth(1, 25);
            
            // الحصول على عرض العمود بالبكسلات
            int widthInPixels = worksheet.Cells.GetColumnWidthPixel(1);
            
            // أخرج النتيجة.
            Console.WriteLine("Column width in pixels: " + widthInPixels);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

يحصل على عرض العمود المحدد في العرض العادي، بوحدة البكسل.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود |
| الأصلي | منطقي | يشير إلى ما إذا كان سيتم إرجاع العرض الأصلي حتى عندما يكون العمود مخفيًا |

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

    public class CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين عرض العمود القياسي إلى 80 بكسل
            worksheet.Cells.StandardWidthPixels = 80;

            // تعيين عرض عمود محدد للعمود 2 (العمود الثالث) إلى 120 بكسل
            worksheet.Cells.SetColumnWidthPixel(2, 120);

            try
            {
                // الحصول على العرض الحالي مع تعديلات المستخدم (original: false)
                int currentWidth = worksheet.Cells.GetColumnWidthPixel(2, false);
                Console.WriteLine($"Column 2 current width: {currentWidth} pixels");

                // الحصول على العرض الأصلي بدون تعديلات (original: true)
                int originalWidth = worksheet.Cells.GetColumnWidthPixel(2, true);
                Console.WriteLine($"Column 2 original width: {originalWidth} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthPixel: {ex.Message}");
            }

            // حفظ المصنف لتوضيح استمرارية عرض العمود
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


