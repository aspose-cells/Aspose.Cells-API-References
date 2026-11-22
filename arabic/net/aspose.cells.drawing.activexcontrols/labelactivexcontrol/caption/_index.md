---
title: "LabelActiveXControl.Caption"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LabelActiveXControl. يحصل ويضبط النص الوصفي الذي يظهر على العنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/caption/
---
## LabelActiveXControl.Caption property

يحصل ويضبط النص الوصفي الذي يظهر على التحكم.

```csharp
public string Caption { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم Label ActiveX
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.Label, 0, 0, 0, 0, 100, 30);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // تعيين وعرض خاصية Caption
            label.Caption = "Label1aaaa";
            
            // احفظ وأعد التحميل للتحقق من الاستمرارية
            string path = "LabelActiveXDemo.xlsm";
            workbook.Save(path, SaveFormat.Xlsm);

            Workbook reopened = new Workbook(path);
            LabelActiveXControl reloadedLabel = (LabelActiveXControl)reopened.Worksheets[0].Shapes[0].ActiveXControl;
            Console.WriteLine("Caption: " + reloadedLabel.Caption);
        }
    }
}
```

### انظر أيضًا

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


