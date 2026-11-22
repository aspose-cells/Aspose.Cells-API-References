---
title: "Column.SetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Column. تحدد النمط لهذا العمود"
type: docs
url: /ar/net/aspose.cells/column/setstyle/
---
## Column.SetStyle method

يضبط نمط هذا العمود.

```csharp
public void SetStyle(Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | النمط الذي سيُستخدم كنمط افتراضي للخلايا في هذا العمود. |

### ملاحظات

هذه الطريقة تقوم فقط بتعيين النمط المحدد كنمط افتراضي لهذا العمود، دون تغيير إعدادات النمط للخلايا الموجودة في هذا العمود. لتحديث إعدادات النمط للخلايا الموجودة إلى النمط المحدد في نفس الوقت، يرجى استخدام [`ApplyStyle`](../applystyle/)

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnMethodSetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى العمود الأول
            Column column = worksheet.Cells.Columns[0];

            // إنشاء نمط جديد من المصنف
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            try
            {
                // تطبيق النمط المخصص على العمود بأكمله
                column.SetStyle(style);
                
                Console.WriteLine($"Style applied successfully to column {column.Index}");
                Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
                Console.WriteLine($"Background: {style.ForegroundColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("ColumnMethodSetStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


