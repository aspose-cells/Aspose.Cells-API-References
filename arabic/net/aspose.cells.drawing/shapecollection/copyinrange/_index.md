---
title: "ShapeCollection.CopyInRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. نسخ الأشكال في النطاق إلى النطاق الوجهة"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

انسخ الأشكال في النطاق إلى النطاق الوجهة.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceShapes | ShapeCollection | الأشكال المصدر. |
| ca | CellArea | النطاق المصدر. |
| destRow | Int32 | فهرس الصف الوجهة للنطاق الوجهة. |
| destColumn | Int32 | عمود الوجهة للنطاق الوجهة. |
| isContained | منطقي | ما إذا كان يجب نسخ الأشكال الموجودة فقط داخل النطاق. إذا كان true، يتم نسخ الأشكال في النطاق فقط. وإلا، يعمل كما في MS Office. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // إضافة شكل مستطيل
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // حدد منطقة الخلايا للنسخ منها
            CellArea area2 = new CellArea();
            area2.StartColumn = 1;
            area2.StartRow = 1;
            area2.EndColumn = 5;
            area2.EndRow = 11;

            // نسخ الأشكال داخل النطاق المحدد
            shapes.CopyInRange(shapes, area2, 12, 1, false);

            // احفظ المصنف
            workbook.Save("ShapeCopyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


