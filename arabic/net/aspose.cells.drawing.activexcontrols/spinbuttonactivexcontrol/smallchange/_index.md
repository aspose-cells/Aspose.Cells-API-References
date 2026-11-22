---
title: "SpinButtonActiveXControl.SmallChange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "SpinButtonActiveXControl خاصية. يحصل ويضبط مقدار التغيير في خاصية Position"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/
---
## SpinButtonActiveXControl.SmallChange property

يحصل على مقدار التغيير في خاصية Position ويضبطه

```csharp
public int SmallChange { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertySmallChangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف SpinButton ActiveX control إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            
            // احصل على عنصر ActiveX واضبط خاصية SmallChange
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.SmallChange = 5;
            
            // احفظ المصنف
            workbook.Save("SpinButtonSmallChangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


