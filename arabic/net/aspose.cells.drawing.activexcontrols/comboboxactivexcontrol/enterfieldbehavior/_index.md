---
title: "ComboBoxActiveXControl.EnterFieldBehavior"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "ComboBoxActiveXControl property. يحدد سلوك التحديد عند دخول العنصر. True يحدد أن التحديد يبقى دون تغيير منذ آخر مرة كان فيها العنصر نشطًا. False يحدد أنه سيتم تحديد كل النص في العنصر عند الدخول إلى العنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/enterfieldbehavior/
---
## ComboBoxActiveXControl.EnterFieldBehavior property

يحدد سلوك الاختيار عند دخول العنصر. True يعني أن الاختيار يبقى دون تغيير منذ آخر مرة كان فيها العنصر نشطًا. False يعني أنه سيتم تحديد كل النص داخل العنصر عند الدخول إليه.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة أول عنصر تحكم ComboBox ActiveX
            Shape shape1 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 50
            );
            ComboBoxActiveXControl combo1 = (ComboBoxActiveXControl)shape1.ActiveXControl;
            combo1.EnterFieldBehavior = false; // Default behavior (select all text on entry)
            combo1.Value = "Select Option";
            combo1.BorderStyle = ControlBorderType.Single;
            
            // إضافة ثاني عنصر تحكم ComboBox ActiveX
            Shape shape2 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 2, 0, 100, 50
            );
            ComboBoxActiveXControl combo2 = (ComboBoxActiveXControl)shape2.ActiveXControl;
            combo2.EnterFieldBehavior = true; // Preserve previous selection
            combo2.Value = "Edit Value";
            combo2.BorderStyle = ControlBorderType.Single;
            
            // احفظ المصنف
            workbook.Save("ComboBoxActiveXControlDemo.xlsm", SaveFormat.Xlsm);
            
            // تحقق من إعدادات الخاصية
            Console.WriteLine("Combo1 EnterFieldBehavior: " + combo1.EnterFieldBehavior);
            Console.WriteLine("Combo2 EnterFieldBehavior: " + combo2.EnterFieldBehavior);
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


