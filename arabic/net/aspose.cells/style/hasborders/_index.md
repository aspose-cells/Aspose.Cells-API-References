---
title: "Style.HasBorders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تتحقق مما إذا تم تعيين حدود للنمط"
type: docs
url: /ar/net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

يتحقق مما إذا تم تعيين حدود للنمط.

```csharp
public bool HasBorders { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHasBordersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // الوصول إلى الخلية A1 والتحقق مما إذا كانت تحتوي على حدود (يجب أن تكون false افتراضيًا)
            Cell cellA1 = cells["A1"];
            Console.WriteLine("Cell A1 has borders: " + cellA1.GetStyle().HasBorders);

            // إنشاء نمط مع حدود
            Style styleWithBorders = workbook.CreateStyle();
            styleWithBorders.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            styleWithBorders.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // تطبيق النمط على الخلية B1
            Cell cellB1 = cells["B1"];
            cellB1.SetStyle(styleWithBorders);

            // تحقق مما إذا كانت الخلية B1 تحتوي على حدود (يجب أن تكون true الآن)
            Console.WriteLine("Cell B1 has borders: " + cellB1.GetStyle().HasBorders);

            // احفظ المصنف
            workbook.Save("HasBordersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


