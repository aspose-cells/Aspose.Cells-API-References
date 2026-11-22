---
title: "ActiveXControlBase.LinkedCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControlBase. تحصل وتضبط الخلية المرتبطة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

يحصل على ويضبط الخلية المرتبطة.

```csharp
public string LinkedCell { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // تهيئة دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة SpinButtonActiveXControl إلى ورقة العمل الأولى
            Aspose.Cells.Drawing.Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 
                10, 10, 100, 30, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;

            // تكوين خصائص زر التدوير
            spinButton.Min = 0;
            spinButton.Max = 100;
            spinButton.Position = 50;
            spinButton.SmallChange = 1;

            // ربط التحكم بالخلية A1
            spinButton.LinkedCell = "A1";

            // تعيين قيمة الخلية A1 لتطابق الموضع الأولي
            workbook.Worksheets[0].Cells["A1"].PutValue(spinButton.Position);

            // احفظ المصنف
            workbook.Save("LinkedCellDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


