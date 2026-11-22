---
title: "ComboBoxActiveXControl.HideSelection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "ComboBoxActiveXControl property. يشير إلى ما إذا كان النص المحدد في العنصر يظهر مميزًا عندما لا يكون للعنصر تركيز"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/hideselection/
---
## ComboBoxActiveXControl.HideSelection property

يشير إلى ما إذا كان النص المحدد في العنصر يظهر مميزًا عندما لا يكون للعنصر تركيز.

```csharp
public bool HideSelection { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ComboBox ActiveX مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // تكوين الخصائص الأساسية
            comboBox.ListRows = 5;
            comboBox.Value = "Select an item";
            
            // إضافة عناصر نموذجية باستخدام اسم الخاصية الصحيح
            comboBox.ListFillRange = "A1:A3"; // Alternative way to set items
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // عرض خاصية HideSelection
            comboBox.HideSelection = true; // Text won't show selection highlight when control loses focus

            // احفظ المصنف
            workbook.Save("ComboBoxHideSelectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


