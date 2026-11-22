---
title: "ActiveXControlBase.Width"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControlBase. تحصل وتضبط عرض التحكم بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/width/
---
## ActiveXControlBase.Width property

يحصل على ويضبط عرض التحكم بوحدة النقاط.

```csharp
public virtual double Width { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            ActiveXControlBase control = (ActiveXControlBase)shape.ActiveXControl;

            // إظهار استخدام خاصية Width
            Console.WriteLine("Original width: " + control.Width);
            control.Width = 150;
            Console.WriteLine("Modified width: " + control.Width);

            workbook.Save("ActiveXControlWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


