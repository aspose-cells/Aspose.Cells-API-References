---
title: "CellsHelper.GetUsedColors"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تحصل على جميع الألوان المستخدمة في المصنف"
type: docs
url: /ar/net/aspose.cells/cellshelper/getusedcolors/
---
## CellsHelper.GetUsedColors method

يحصل على جميع الألوان المستخدمة في دفتر العمل.

```csharp
public static Color[] GetUsedColors(Workbook workbook)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصنف | المصنف | كائن المصنف. |

### قيمة الإرجاع

الألوان المستخدمة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsHelperMethodGetUsedColorsWithWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض الخلايا الملونة لتوضيح الألوان المستخدمة
            worksheet.Cells["A1"].PutValue("Red Cell");
            worksheet.Cells["A1"].GetStyle().ForegroundColor = Color.Red;
            worksheet.Cells["A1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["A1"].SetStyle(worksheet.Cells["A1"].GetStyle());

            worksheet.Cells["B1"].PutValue("Blue Cell");
            worksheet.Cells["B1"].GetStyle().ForegroundColor = Color.Blue;
            worksheet.Cells["B1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["B1"].SetStyle(worksheet.Cells["B1"].GetStyle());

            worksheet.Cells["C1"].PutValue("Green Cell");
            worksheet.Cells["C1"].GetStyle().ForegroundColor = Color.Green;
            worksheet.Cells["C1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["C1"].SetStyle(worksheet.Cells["C1"].GetStyle());

            try
            {
                // استدعِ طريقة GetUsedColors مع معامل المصنف
                Color[] usedColors = CellsHelper.GetUsedColors(workbook);

                // عرض الألوان المستخدمة
                Console.WriteLine("Used colors in the workbook:");
                foreach (Color color in usedColors)
                {
                    Console.WriteLine($"Color: A={color.A}, R={color.R}, G={color.G}, B={color.B}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetUsedColors method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("CellsHelperGetUsedColorsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../workbook/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


