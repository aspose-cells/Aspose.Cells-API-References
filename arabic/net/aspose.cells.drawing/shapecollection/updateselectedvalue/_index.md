---
title: "ShapeCollection.UpdateSelectedValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تحديث القيمة المحددة بقيمة الخلية المرتبطة أو نطاق الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

حدّث القيمة المحددة بقيمة الخلية المرتبطة أو نطاق الشكل.

```csharp
public void UpdateSelectedValue()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل (قائمة منسدلة) إلى ورقة العمل
            Aspose.Cells.Drawing.ListBox listBox = (Aspose.Cells.Drawing.ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 3, 20);
            
            // تعيين عناصر القائمة والقيمة المحددة
            listBox.SetInputRange("A1:A3", false, false);
            listBox.SelectedIndex = 1;
            
            // تحديث القيمة المحددة في الشكل
            worksheet.Shapes.UpdateSelectedValue();
            
            // احفظ المصنف
            workbook.Save("ShapeCollectionUpdateSelectedValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


