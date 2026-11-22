---
title: "ActiveXControlBase.IsVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControlBase. تشير إلى ما إذا كان هذا العنصر مرئيًا"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/
---
## ActiveXControlBase.IsVisible property

يشير إلى ما إذا كان هذا التحكم مرئياً.

```csharp
public virtual bool IsVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر ListBox ActiveX control
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 1, 100, 100);
            var listBox = shape.ActiveXControl;

            // تكوين الخصائص الأساسية
            listBox.IsVisible = true; // Demonstrate IsVisible property
            Console.WriteLine("Initial visibility: " + listBox.IsVisible);
            listBox.IsVisible = false;
            Console.WriteLine("After setting to false: " + listBox.IsVisible);
            listBox.IsVisible = true;
            Console.WriteLine("After setting to true: " + listBox.IsVisible);

            // احفظ المصنف
            workbook.Save("ActiveXControlVisibilityDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


