---
title: "Style.Borders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل على BorderCollection للنمط"
type: docs
url: /ar/net/aspose.cells/style/borders/
---
## Style.Borders property

يحصل على [`BorderCollection`](../../bordercollection/) للنمط.

```csharp
public BorderCollection Borders { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBordersDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الحصول على الخلية ونمطها
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // تعيين أنماط حدود مختلفة
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            
            // تطبيق النمط على الخلية
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("BorderStylesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


