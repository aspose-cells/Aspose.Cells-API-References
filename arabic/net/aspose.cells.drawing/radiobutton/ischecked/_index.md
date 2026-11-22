---
title: "RadioButton.IsChecked"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RadioButton. تشير إلى ما إذا كان زر الاختيار محددًا أم لا"
type: docs
url: /ar/net/aspose.cells.drawing/radiobutton/ischecked/
---
## RadioButton.IsChecked property

يشير إلى ما إذا كان زر الاختيار محددًا أم لا.

```csharp
public bool IsChecked { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonPropertyIsCheckedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة زر اختيار إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 100);
            RadioButton radioButton = (RadioButton)shape;
            
            // تعيين نص زر الاختيار
            radioButton.Text = "Option 1";
            
            // غير محدد في البداية
            radioButton.IsChecked = false;
            Console.WriteLine("Radio button initially unchecked: " + radioButton.IsChecked);
            
            // تحديد زر الاختيار
            radioButton.IsChecked = true;
            Console.WriteLine("Radio button after checking: " + radioButton.IsChecked);
            
            // احفظ المصنف
            workbook.Save("RadioButtonExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


