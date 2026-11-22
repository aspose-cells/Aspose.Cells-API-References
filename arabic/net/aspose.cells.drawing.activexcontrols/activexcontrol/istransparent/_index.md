---
title: "ActiveXControl.IsTransparent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControl. تشير إلى ما إذا كان التحكم شفافًا"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

يشير إلى ما إذا كان العنصر شفافًا.

```csharp
public bool IsTransparent { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsTransparentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لاستضافة عنصر تحكم ActiveX مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 200, 50, 
                0, 0); // Adding missing parameters for upperLeftRow, upperLeftColumn, height, width, left, top

            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // تعيين خصائص التحكم
            label.Caption = "Sample Label";
            label.IsTransparent = false; // Demonstrating IsTransparent property

            // التحقق وإخراج خاصية IsTransparent
            Console.WriteLine("Label IsTransparent property: " + label.IsTransparent);

            // تغيير الشفافية والتحقق مرة أخرى
            label.IsTransparent = true;
            Console.WriteLine("Label IsTransparent property after change: " + label.IsTransparent);

            // احفظ المصنف
            workbook.Save("ActiveXControlIsTransparentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


