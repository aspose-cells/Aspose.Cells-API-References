---
title: "ShapeCollection.AddPicture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تضيف صورة إلى المجموعة"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addpicture/
---
## AddPicture(int, int, int, int, Stream) {#addpicture}

يضيف صورة إلى المجموعة.

```csharp
public Picture AddPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| الصف السفلي | Int32 | فهرس الصف السفلي الأيمن |
| rightColumn | Int32 | فهرس العمود السفلي الأيمن |
| تدفق | Stream | كائن Stream الذي يحتوي على بيانات الصورة. |

### قيمة الإرجاع

[`Picture`](../../picture/) Picture object.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddPictureWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // إضافة صورة من تدفق ملف
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                Picture picture = shapes.AddPicture(1, 0, 1, 0, fs);
            }

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddPicture(int, int, Stream, int, int) {#addpicture_1}

يضيف صورة إلى المجموعة.

```csharp
public Picture AddPicture(int topRow, int leftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| تدفق | Stream | كائن Stream الذي يحتوي على بيانات الصورة. |
| widthScale | Int32 | مقياس عرض الصورة، نسبة مئوية. |
| heightScale | Int32 | مقياس ارتفاع الصورة، نسبة مئوية. |

### قيمة الإرجاع

[`Picture`](../../picture/) Picture object.

### أمثلة

```csharp

[C#]
//إضافة صورة
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    Picture picture = shapes.AddPicture(1, 1, fs, 50, 60);
}
```

### انظر أيضًا

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


