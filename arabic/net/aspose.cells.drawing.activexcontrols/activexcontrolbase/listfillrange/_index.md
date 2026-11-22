---
title: "ActiveXControlBase.ListFillRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControlBase. يسترجع ويضبط نطاق تعبئة القائمة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/
---
## ActiveXControlBase.ListFillRange property

يحصل على ويضبط نطاق تعبئة القائمة.

```csharp
public string ListFillRange { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyListFillRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لـ ListFillRange
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
            }

            // أضف ComboBoxActiveXControl
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1, 0, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // عيّن ListFillRange لملء صندوق القوائم
            comboBox.ListFillRange = "A2:A10";

            // احفظ المصنف
            workbook.Save("ActiveXControlListFillRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


