---
title: "ShapeCollection.DeleteInRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. حذف الأشكال في النطاق. لن يتم حذف أشكال التعليق"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

احذف الأشكال في النطاق. لن يتم حذف أشكال التعليقات.

```csharp
public void DeleteInRange(CellArea ca)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | النطاق. إذا كانت الأشكال موجودة في النطاق، فسيتم إزالتها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteInRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // إضافة الشكل المستطيل الأول
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // إضافة الشكل المستطيل الثاني
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // تحديد النطاق الذي يجب حذف الأشكال فيه
            CellArea area = new CellArea();
            area.StartColumn = 0;
            area.StartRow = 5;
            area.EndColumn = 5;
            area.EndRow = 8;

            // حذف الأشكال داخل النطاق المحدد
            shapes.DeleteInRange(area);

            // احفظ دفتر العمل (اختياري)
            workbook.Save("ShapeDeleteInRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


