---
title: "ListBoxActiveXControl.BorderOleColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBoxActiveXControl. تحصل وتحدد لون ole للخلفية"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderolecolor/
---
## ListBoxActiveXControl.BorderOleColor property

يحصل ويضبط لون الـole للخلفية.

```csharp
public int BorderOleColor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 0, 0, 200, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
            
            listBox.BorderOleColor = -2147483642;
            
            workbook.Save("ListBoxBorderOleColorDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### انظر أيضًا

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


