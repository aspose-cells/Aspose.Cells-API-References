---
title: "ShapeCollection.AddActiveXControl"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تُنشئ عنصر تحكم Activex"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addactivexcontrol/
---
## ShapeCollection.AddActiveXControl method

ينشئ عنصر تحكم Activex.

```csharp
public Shape AddActiveXControl(ControlType type, int topRow, int top, int leftColumn, int left, 
    int width, int height)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ControlType | نوع التحكم. |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع الشكل، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض الشكل، بوحدة البكسل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddActiveXControlWithControlTypeInt32Int32Int32Int3Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape activeXControl = shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 
                1,  // upperLeftRow
                0,  // top
                1,  // upperLeftColumn
                0,  // left
                100,  // width
                50   // height
            );

            workbook.Save("AddActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


