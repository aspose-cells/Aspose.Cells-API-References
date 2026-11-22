---
title: "Border.LineStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Border. يحصل على أو يضبط نوع حد الخلية"
type: docs
url: /ar/net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

يحصل أو يضبط نوع حد الخلية.

```csharp
public CellBorderType LineStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyLineStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى خلية والحصول على نمطها
            Cell cell = worksheet.Cells["B2"];
            Style style = cell.GetStyle();

            // ضبط أنماط خطوط حدود مختلفة
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;

            // تطبيق النمط على الخلية
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("BorderLineStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


