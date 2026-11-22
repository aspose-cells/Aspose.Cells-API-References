---
title: "ListBoxActiveXControl.IntegralHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBoxActiveXControl. تشير إلى ما إذا كان التحكم سيعرض فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/integralheight/
---
## ListBoxActiveXControl.IntegralHeight property

يُشير إلى ما إذا كان العنصر سيعرض فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية.

```csharp
public bool IntegralHeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyIntegralHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,
                10,  // left
                10,  // top
                200, // width
                100, // height
                0,   // imageWidth (required parameter)
                0    // imageHeight (required parameter)
            );
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // اعرض خاصية IntegralHeight
            listBox.IntegralHeight = true;
            Console.WriteLine("ListBox IntegralHeight set to: " + listBox.IntegralHeight);

            // أضف عناصر نموذجية
            listBox.ListFillRange = "A1:A3";
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            workbook.Save("ListBoxIntegralHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


