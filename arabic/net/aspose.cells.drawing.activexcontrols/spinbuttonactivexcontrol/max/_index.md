---
title: "SpinButtonActiveXControl.Max"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "SpinButtonActiveXControl خاصية. يحصل ويضبط القيمة القصوى المقبولة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/
---
## SpinButtonActiveXControl.Max property

يحصل على ويضبط القيمة القصوى المقبولة.

```csharp
public int Max { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMaxDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف SpinButton ActiveX control إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 1, 1, 1, 100, 30);
            
            // احصل على عنصر ActiveX واضبط خاصية Max الخاصة به
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Max = 100;
            
            // احفظ المصنف
            workbook.Save("SpinButtonMaxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


