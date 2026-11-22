---
title: "Cells.UngroupRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تفك تجميع الصفوف"
type: docs
url: /ar/net/aspose.cells/cells/ungrouprows/
---
## UngroupRows(int, int, bool) {#ungrouprows_1}

يفك تجميع الصفوف.

```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | Int32 | مؤشر الصف الأول الذي سيتم فك تجميعه. |
| lastIndex | Int32 | مؤشر الصف الأخير الذي سيتم فك تجميعه. |
| isAll | منطقي | True، يزيل جميع معلومات التجميع. وإلا، يزيل معلومات المجموعة الخارجية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUngroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء تجميعات صفوف متداخلة للتوضيح
            worksheet.Cells.GroupRows(5, 7);  // First level grouping
            worksheet.Cells.GroupRows(5, 7);  // Second level grouping

            try
            {
                // فك تجميع جميع مستويات الصفوف 5-7
                worksheet.Cells.UngroupRows(5, 7, true);

                Console.WriteLine("Rows 5-7 successfully ungrouped with all levels removed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UngroupRows: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("UngroupRowsWithBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## UngroupRows(int, int) {#ungrouprows}

يفك تجميع الصفوف.

```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | Int32 | مؤشر الصف الأول الذي سيتم فك تجميعه. |
| lastIndex | Int32 | مؤشر الصف الأخير الذي سيتم فك تجميعه. |

### ملاحظات

يزيل فقط معلومات المجموعة الخارجية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ملء بعض البيانات
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue($"Row {i}");
            }

            // تجميع الصفوف من 1 إلى 3 (فهرس يبدأ من 0)
            cells.GroupRows(1, 3, true);

            Console.WriteLine("Rows grouped from index 1 to 3");

            // فك تجميع نفس الصفوف
            cells.UngroupRows(1, 3);

            Console.WriteLine("Rows ungrouped from index 1 to 3");

            // احفظ المصنف
            workbook.Save("UngroupRowsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


