---
title: "ListBoxActiveXControl.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBoxActiveXControl. تحصل على نوع التحكم ActiveX"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/type/
---
## ListBoxActiveXControl.Type property

يحصل على نوع عنصر التحكم ActiveX.

```csharp
public override ControlType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف عنصر تحكم ListBox ActiveX مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 0, 0);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
            
            // عرض خاصية Type
            Console.WriteLine("Control Type: " + listBox.Type);
            
            // تعيين بعض الخصائص
            listBox.ScrollBars = ControlScrollBarType.BarsBoth;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
            listBox.ListStyle = ControlListStyle.Plain;
            listBox.SelectionType = SelectionType.Single;
            
            // تحقق من خاصية Type
            if (listBox.Type == ControlType.ListBox)
            {
                Console.WriteLine("This is a ListBox control as expected");
            }
            
            // احفظ المصنف
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlType](../../controltype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


