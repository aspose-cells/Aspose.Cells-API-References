---
title: "ListBoxActiveXControl.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBoxActiveXControl. تحصل وتضبط قيمة العنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/value/
---
## ListBoxActiveXControl.Value property

يحصل على قيمة التحكم ويضبطها.

```csharp
public string Value { get; set; }
```

### ملاحظات

يؤثر فقط عندما يكون [`SelectionType`](../selectiontype/) هو SelectionType.Single;

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر ListBox ActiveX control
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // تعيين الخصائص الأساسية
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;

            // اضبط العناصر باستخدام خاصية Value
            listBox.Value = "Red;Green;Blue;Yellow";

            // احفظ المصنف
            workbook.Save("ListBoxValueDemo.xlsx");

            Console.WriteLine("ListBox with items set using Value property has been created.");
        }
    }
}
```

### انظر أيضًا

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


