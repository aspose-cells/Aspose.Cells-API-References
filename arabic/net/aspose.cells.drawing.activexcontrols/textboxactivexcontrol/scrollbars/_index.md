---
title: "TextBoxActiveXControl.ScrollBars"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تحدد ما إذا كان العنصر يحتوي على أشرطة تمرير عمودية أو أشرطة تمرير أفقية أو كليهما أو لا شيء"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/
---
## TextBoxActiveXControl.ScrollBars property

يشير إلى ما إذا كان العنصر يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كليهما، أو لا شيء.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء مجموعة أشكال جديدة وإضافة عنصر ActiveX
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
            
            // اضبط خاصية ScrollBars إلى عمودي
            textBox.ScrollBars = ControlScrollBarType.BarsVertical;
            
            // احفظ المصنف
            workbook.Save("TextBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


