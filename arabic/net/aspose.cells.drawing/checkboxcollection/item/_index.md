---
title: "CheckBoxCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CheckBoxCollection. يحصل على عنصر CheckBox في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/checkboxcollection/item/
---
## CheckBoxCollection indexer

يحصل على العنصر [`CheckBox`](../../checkbox/) في الفهرس المحدد.

```csharp
public CheckBox this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة خانة اختيار إلى ورقة العمل
            int index = worksheet.CheckBoxes.Add(10, 10, 100, 20);
            
            // الوصول إلى checkBox باستخدام خاصية Item (المؤشر)
            Aspose.Cells.Drawing.CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Name = "CheckBox1";
            
            // الوصول إلى checkBox باستخدام الفهرس (خاصية Item)
            Aspose.Cells.Drawing.CheckBox checkBoxByName = worksheet.CheckBoxes[0];
            
            // إخراج خصائص checkBox
            Console.WriteLine("CheckBox Name: " + checkBoxByName.Name);
            Console.WriteLine("CheckBox Text: " + checkBoxByName.Text);
            
            // احفظ المصنف
            workbook.Save("CheckBoxExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


