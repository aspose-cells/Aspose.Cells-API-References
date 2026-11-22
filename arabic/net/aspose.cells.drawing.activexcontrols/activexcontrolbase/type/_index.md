---
title: "ActiveXControlBase.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControlBase. يسترجع نوع عنصر ActiveX"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/type/
---
## ActiveXControlBase.Type property

يحصل على نوع عنصر التحكم ActiveX.

```csharp
public abstract ControlType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم Label ActiveX مع المعلمات الصحيحة
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 100, 50, 0);
            LabelActiveXControl labelControl = (LabelActiveXControl)labelShape.ActiveXControl;
            labelControl.Caption = "Label_ActiveX";

            // توضيح استخدام خاصية Type
            if (labelShape.ActiveXControl.Type == ControlType.Label)
            {
                Console.WriteLine("The control is a Label type");
                labelControl.Caption = labelControl.Caption.Replace("Label_", "MyChangedLabel_");
            }

            // حفظ والتحقق
            workbook.Save("output.xlsx");
            Console.WriteLine("Label caption changed to: " + labelControl.Caption);
        }
    }
}
```

### انظر أيضًا

* enum [ControlType](../../controltype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


