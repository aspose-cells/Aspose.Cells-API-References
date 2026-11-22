---
title: "ShapeCollection.AddAutoShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تضيف AutoShape إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

يضيف AutoShape إلى ورقة العمل.

```csharp
public Shape AddAutoShape(AutoShapeType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | AutoShapeType | نوع الشكل التلقائي. |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع الشكل، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض الشكل، بوحدة البكسل. |

### قيمة الإرجاع

كائن Shape.

### ملاحظات

النوع لا يمكن أن يكون Chart/Comment/Picture/OleObject/Polygon/DialogBox

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddAutoShapeWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
            
            workbook.Save("AutoShapeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


