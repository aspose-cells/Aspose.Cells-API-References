---
title: "Cells.ShowGroupDetail"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. توسع الصفوف/الأعمدة المجمعة"
type: docs
url: /ar/net/aspose.cells/cells/showgroupdetail/
---
## Cells.ShowGroupDetail method

يوسع الصفوف/الأعمدة المجمعة.

```csharp
public void ShowGroupDetail(bool isVertical, int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isVertical | منطقي | صحيح، يوسع الصفوف المجمعة. |
| فهرس | Int32 | مؤشر الصف/العمود |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodShowGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ بيانات العينة في الصفوف 5-7 (فهرس صفرية 4-6)
            for (int row = 4; row <= 6; row++)
            {
                worksheet.Cells[row, 0].PutValue($"Row {row + 1}");
            }

            // تجميع الصفوف 4-6 (صفوف Excel 5-7) وطيها مبدئياً
            worksheet.Cells.GroupRows(4, 6, true);

            try
            {
                // توسيع الصفوف المجمعة باستخدام ShowGroupDetail (isVertical: false للصفوف، الفهرس: 4)
                worksheet.Cells.ShowGroupDetail(false, 4);
                Console.WriteLine("ShowGroupDetail method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShowGroupDetail: {ex.Message}");
            }

            // احفظ المصنف لتوضيح التأثير
            workbook.Save("ShowGroupDetailWithBooleanInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


