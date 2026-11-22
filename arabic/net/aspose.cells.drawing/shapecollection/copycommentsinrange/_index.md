---
title: "ShapeCollection.CopyCommentsInRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. نسخ جميع التعليقات في النطاق"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
## ShapeCollection.CopyCommentsInRange method

انسخ جميع التعليقات في النطاق.

```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الأشكال | ShapeCollection | الأشكال المصدر. |
| ca | CellArea | النطاق المصدر. |
| destRow | Int32 | صف البداية للنطاق الوجهة. |
| destColumn | Int32 | عمود البداية للنطاق الوجهة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyCommentsInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليقات
            CommentCollection comments = worksheet.Comments;
            
            // إضافة تعليق إلى الخلية A1
            int commentIndex = comments.Add(0, 0);
            Comment comment = comments[commentIndex];
            comment.Note = "First note.";
            comment.Font.Name = "Times New Roman";
            
            // إضافة تعليق إلى الخلية B2
            comments.Add("B2");
            comment = comments["B2"];
            comment.Note = "Second note.";
            
            // تحديد النطاق المصدر
            CellArea sourceArea = new CellArea();
            sourceArea.StartRow = 0;
            sourceArea.StartColumn = 0;
            sourceArea.EndRow = 1;
            sourceArea.EndColumn = 1;
            
            // الحصول على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;
            
            // نسخ التعليقات من النطاق المصدر إلى الوجهة (بدءًا من الصف 5، العمود 1)
            shapes.CopyCommentsInRange(shapes, sourceArea, 5, 1);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


