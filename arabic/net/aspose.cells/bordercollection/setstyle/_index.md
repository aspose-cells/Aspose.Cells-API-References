---
title: "BorderCollection.SetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة BorderCollection. تعيين نمط جميع حدود المجموعة"
type: docs
url: /ar/net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

يضبط نمط جميع حدود المجموعة.

```csharp
public void SetStyle(CellBorderType style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | CellBorderType | نمط الحدود |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetStyleWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على الخلية C6 ونمطها
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();

            // حدد لون الحدود والنمط
            style.Borders.SetColor(System.Drawing.Color.Red);
            style.Borders.SetStyle(CellBorderType.Thick);

            // تطبيق النمط على الخلية
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("BorderCollectionMethodSetStyleWithCellBorderTypeDemo_out.xlsx");

            Console.WriteLine("Border style set successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


