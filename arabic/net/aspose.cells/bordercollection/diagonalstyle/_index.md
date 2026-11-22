---
title: "BorderCollection.DiagonalStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BorderCollection. تحصل أو تعين نمط الخطوط القطرية"
type: docs
url: /ar/net/aspose.cells/bordercollection/diagonalstyle/
---
## BorderCollection.DiagonalStyle property

يحصل أو يضبط نمط الخطوط القطرية.

```csharp
public CellBorderType DiagonalStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على خلية ونمطها
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // حدد خصائص الحدود القطرية
            style.Borders.DiagonalStyle = CellBorderType.Thin;
            style.Borders.DiagonalColor = Color.Red;
            
            // تطبيق النمط على الخلية
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


