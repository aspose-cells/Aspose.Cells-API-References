---
title: "ScrollBarActiveXControl.LargeChange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScrollBarActiveXControl. تحصل وتضبط مقدار التغيير في خاصية Position"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/largechange/
---
## ScrollBarActiveXControl.LargeChange property

يحصل على مقدار التغيير في خاصية Position ويضبطه

```csharp
public int LargeChange { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyLargeChangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ScrollBar ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 30);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // ضبط خاصية LargeChange
            scrollBar.LargeChange = 5;

            // احفظ المصنف
            workbook.Save("ScrollBarActiveXControlLargeChangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


