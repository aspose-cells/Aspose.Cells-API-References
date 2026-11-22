---
title: "SpinButtonActiveXControl.Min"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SpinButtonActiveXControl. تسترجع وتضبط الحد الأدنى للقيمة المقبولة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/
---
## SpinButtonActiveXControl.Min property

يحصل على ويضبط القيمة الدنيا المقبولة.

```csharp
public int Min { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMinDemo
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
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            
            // عيّن خاصية Min لعنصر SpinButton
            spinButton.Min = 0;
            
            // اضبط خصائص أخرى لتوضيح الوظيفة
            spinButton.Max = 100;
            spinButton.Position = 50;
            
            // احفظ المصنف
            workbook.Save("SpinButtonMinDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


