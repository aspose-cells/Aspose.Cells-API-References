---
title: "ShapeCollection.AddCopy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يضيف وينسخ شكلًا إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addcopy/
---
## AddCopy(Shape, int, int, int, int) {#addcopy}

يضيف وينسخ شكلاً إلى ورقة العمل.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceShape | شكل | الشكل المصدر. |
| topRow | Int32 | فهرس الصف العلوي. |
| أعلى | Int32 | يمثل الإزاحة العمودية من صفه العلوي، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية من عموده الأيسر، بوحدة البكسل. |

### قيمة الإرجاع

الكائن الجديد [`Shape`](../../shape/).

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCopyWithShapeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // إضافة شكل مستطيل
            RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // أضف نسخة من الشكل المستطيل بموقع جديد
            shapes.AddCopy(rectangle, 7, 0, 7, 0);

            // احفظ المصنف
            workbook.Save("ShapeCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Shape, int, int, int, int, CopyOptions) {#addcopy_1}

يضيف وينسخ شكلاً إلى ورقة العمل.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, 
    CopyOptions copyOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceShape | شكل | الشكل المصدر. |
| topRow | Int32 | فهرس الصف العلوي. |
| أعلى | Int32 | يمثل الإزاحة العمودية من صفه العلوي، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية من عموده الأيسر، بوحدة البكسل. |
| copyOptions | CopyOptions | خيارات نسخ الأشكال. |

### قيمة الإرجاع

الكائن الجديد [`Shape`](../../shape/).

### أمثلة

```csharp

[C#]
//أضف شكلاً
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//يضيف وينسخ شكلاً.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### انظر أيضًا

* class [Shape](../../shape/)
* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


