---
title: "TextBoxActiveXControl.IsAutoWordSelected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تحدد الوحدة الأساسية المستخدمة لتوسيع التحديد. true يعني أن الوحدة الأساسية هي حرف واحد. false يعني أن الوحدة الأساسية هي كلمة كاملة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautowordselected/
---
## TextBoxActiveXControl.IsAutoWordSelected property

يحدد الوحدة الأساسية المستخدمة لتوسيع الاختيار. True يعني أن الوحدة الأساسية هي حرف واحد. false يعني أن الوحدة الأساسية هي كلمة كاملة.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 0, 0, 1, 1, 200, 30);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)textBoxShape.ActiveXControl;

            Console.WriteLine("Initial IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);

            if (!textBoxControl.IsAutoWordSelected)
            {
                textBoxControl.IsAutoWordSelected = true;
            }

            Console.WriteLine("Final IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);
        }
    }
}
```

### انظر أيضًا

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


