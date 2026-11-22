---
title: "ActiveXControlBase.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControlBase. يسترجع ويضبط ارتفاع العنصر بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/height/
---
## ActiveXControlBase.Height property

يحصل على ويضبط ارتفاع التحكم بوحدة النقاط.

```csharp
public virtual double Height { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyHeightDemo
    {
        public static void Run()
        {
            // تهيئة دفتر عمل جديد
            Workbook workbook = new Workbook();

            // أضف RadioButton ActiveXControl
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 50);
            RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.ActiveXControl;

            // تعيين الخصائص الأساسية
            activeXControl.Caption = "Height Demo";
            activeXControl.IsAutoSize = false; // Disable auto-size to demonstrate Height property

            // عرض خاصية Height
            Console.WriteLine("Original Height: " + activeXControl.Height);
            activeXControl.Height = 75;
            Console.WriteLine("Modified Height: " + activeXControl.Height);

            // احفظ المصنف
            workbook.Save("ActiveXControlHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


