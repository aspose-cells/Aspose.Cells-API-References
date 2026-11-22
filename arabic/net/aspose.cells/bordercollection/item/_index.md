---
title: "BorderCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BorderCollection. تحصل على عنصر Border عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/bordercollection/item/
---
## BorderCollection indexer

يحصل على عنصر [`Border`](../../border/) عند الفهرس المحدد.

```csharp
public Border this[BorderType borderType] { get; }
```

| معامل | الوصف |
| --- | --- |
| borderType | الحد الذي سيتم استرجاعه. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // احصل على الخلية ونمطها
                Cell cell = worksheet.Cells["A1"];
                Style style = cell.GetStyle();

                // الوصول إلى BorderCollection من النمط
                BorderCollection borders = style.Borders;

                // عرض القيمة الحالية لخاصية Item (عملية قراءة)
                // ملاحظة: خاصية Item للقراءة فقط وتعيد كائن Border
                // خاصية Item تتطلب معامل BorderType
                Border border = borders[BorderType.LeftBorder];
                Console.WriteLine("Border type: " + border.LineStyle);
                Console.WriteLine("Border color: " + border.Color);

                // حفظ النتيجة
                workbook.Save("ItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated");
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

* class [Border](../../border/)
* enum [BorderType](../../bordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


