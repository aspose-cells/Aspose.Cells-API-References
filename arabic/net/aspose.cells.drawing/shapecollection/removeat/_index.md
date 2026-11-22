---
title: "ShapeCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. إزالة الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection.RemoveAt method

أزل الشكل.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس الشكل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // إضافة الشكل المستطيل الأول
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // إضافة الشكل المستطيل الثاني
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // إزالة الشكل الأول عند الفهرس 0
            shapes.RemoveAt(0);

            // احفظ المصنف
            workbook.Save("ShapeCollectionRemoveAtDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


