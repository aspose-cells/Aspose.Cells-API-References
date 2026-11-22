---
title: "Picture.Move"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Picture. تنقل الصورة إلى موقع محدد"
type: docs
url: /ar/net/aspose.cells.drawing/picture/move/
---
## Picture.Move method

ينقل الصورة إلى موقع محدد.

```csharp
public void Move(int topRow, int leftColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            pic.Move(2, 4);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


