---
title: "ActiveXControlBase.ForeOleColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControlBase. تحصل وتضبط لون OLE للواجهة الأمامية"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/
---
## ActiveXControlBase.ForeOleColor property

يحصل على ويضبط لون OLE للمقدمة.

```csharp
public virtual int ForeOleColor { get; set; }
```

### ملاحظات

لا ينطبق على التحكم Image.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyForeOleColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم CheckBox ActiveX مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // تعيين الخصائص الأساسية
            checkBox.Caption = "Sample CheckBox";
            checkBox.IsAutoSize = true;

            // عرض خاصية ForeOleColor
            checkBox.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            checkBox.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);

            // احفظ المصنف
            workbook.Save("ActiveXControlForeOleColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


