---
title: "ShapeCollection.AddScrollBar"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تضيف ScrollBar إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addscrollbar/
---
## ShapeCollection.AddScrollBar method

يضيف ScrollBar إلى ورقة العمل.

```csharp
public ScrollBar AddScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية لـ ScrollBar من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية لـ ScrollBar من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع ScrollBar، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض ScrollBar، بوحدة البكسل. |

### قيمة الإرجاع

كائن ScrollBar.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddScrollBarWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            ScrollBar scrollBar = shapes.AddScrollBar(1, 0, 100, 20, 0, 100);
            scrollBar.CurrentValue = 50;
            scrollBar.Width = 200;
            scrollBar.Height = 30;

            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScrollBar](../../scrollbar/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


