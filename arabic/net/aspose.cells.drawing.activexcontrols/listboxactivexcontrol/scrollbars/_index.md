---
title: "ListBoxActiveXControl.ScrollBars"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBoxActiveXControl. تشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية أو أشرطة تمرير أفقية أو كليهما أو لا شيء"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/scrollbars/
---
## ListBoxActiveXControl.ScrollBars property

يشير إلى ما إذا كان العنصر يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كليهما، أو لا شيء.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBoxControl = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // أضف بعض العناصر لجعل أشرطة التمرير مرئية
            listBoxControl.ListFillRange = "A1:A20";
            for (int i = 1; i <= 20; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }

            // إظهار خاصية ScrollBars
            listBoxControl.ScrollBars = Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType.BarsBoth;

            workbook.Save("ListBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


