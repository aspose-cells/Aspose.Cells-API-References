---
title: "ToggleButtonActiveXControl.Accelerator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ToggleButtonActiveXControl. تحصل وتضبط مفتاح الاختصار للعنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator/
---
## ToggleButtonActiveXControl.Accelerator property

يحصل ويضبط مفتاح الاختصار للتحكم.

```csharp
public char Accelerator { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ToggleButton ActiveX مع المعلمات المناسبة
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // قم بتعيين خاصية Accelerator
            toggleButton.Accelerator = 'A';
            Console.WriteLine("ToggleButton Accelerator set to: " + toggleButton.Accelerator);

            // امسح خاصية Accelerator
            toggleButton.Accelerator = '\0';
            Console.WriteLine("ToggleButton Accelerator cleared: " + (toggleButton.Accelerator == '\0' ? "True" : "False"));
        }
    }
}
```

### انظر أيضًا

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


