---
title: "ShapeCollection.AddFreeform"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تضيف شكلاً حرًا إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

يضيف شكلاً حرًا إلى ورقة العمل.

```csharp
public Shape AddFreeform(int topRow, int top, int leftColumn, int left, int height, int width, 
    ShapePath[] paths)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية للشكل الحر من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية للشكل الحر من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع الشكل الحر، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض الشكل الحر، بوحدة البكسل. |
| مسارات | ShapePath[] | يمثل مسارًا معرفًا من قبل المستخدم |

### قيمة الإرجاع

شكل حر.

### ملاحظات

ملاحظة: أن العرض والارتفاع في المعلمات يمكن أن يكونا أي قيم صحيحة موجبة، وليس العرض والارتفاع الكليين لمصفوفة ShapePath المحددة بـ ’paths'. العلاقة بينهما هي علاقة مملوءة بمقياس، أي أن كل كائن ShapePath سيتم تحجيمه وفقًا للعرض والارتفاع. لذلك، عندما يكون هناك عدة كائنات في 'paths'، يجب تصميم كل كائن ShapePath بشكل معقول لتلبية التوقعات. عندما يكون هناك كائن ShapePath واحد ولا توجد متطلبات أخرى، فإن تمرير عرض وارتفاع الكائن كقيم للمعاملات يُعد حلاً جيدًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeformWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // إنشاء مسارات أشكال مخصصة
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                                96.5f, -7.148871f,
                                130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                                182.24997f, 75.351f,
                                201, 120.517795f);
            shapePath1.MoveTo(150, 80);
            shapePath1.ArcTo(25, 25, 0, 270);
            
            // إضافة شكل حر إلى ورقة العمل
            shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1 });

            // احفظ المصنف
            workbook.Save("AddFreeformDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


