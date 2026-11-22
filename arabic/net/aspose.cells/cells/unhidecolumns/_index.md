---
title: "Cells.UnhideColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. إظهار عدة أعمدة"
type: docs
url: /ar/net/aspose.cells/cells/unhidecolumns/
---
## Cells.UnhideColumns method

يكشف عن عدة أعمدة.

```csharp
public void UnhideColumns(int column, int totalColumns, double width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |
| totalColumns | Int32 | رقم العمود |
| العرض | Double | عرض العمود. |

### ملاحظات

يطبق عرض العمود فقط على الأعمدة المخفية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUnhideColumnsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إخفاء الأعمدة 1-3 (بدءًا من الصفر) في البداية
            worksheet.Cells.HideColumns(1, 3);

            try
            {
                // إظهار الأعمدة بدءًا من الفهرس 1 (العمود الثاني)، عرض 3 أعمدة، وتعيين العرض إلى 15.5
                worksheet.Cells.UnhideColumns(1, 3, 15.5);

                // تحقق من الأعمدة المكشوفة بفحص عرضها
                Console.WriteLine($"Column 1 width after unhiding: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine("Columns 1-3 successfully unhidden with specified width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnhideColumns: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("UnhideColumnsWithWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


