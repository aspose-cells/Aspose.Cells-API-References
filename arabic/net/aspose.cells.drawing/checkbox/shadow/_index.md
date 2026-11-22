---
title: "CheckBox.Shadow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CheckBox. تشير إلى ما إذا كان صندوق القائمة يحتوي على تظليل ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

يشير إلى ما إذا كان صندوق الجمع يحتوي على تظليل ثلاثي الأبعاد.

```csharp
public bool Shadow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف مربع اختيار إلى ورقة العمل واحصل على فهرسه
            int checkBoxIndex = sheet.CheckBoxes.Add(1, 1, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            
            // تكوين خصائص مربع الاختيار
            checkBox.Text = "Enable Feature";
            checkBox.Value = true;
            
            // عرض خاصية Shadow
            checkBox.Shadow = true; // Enable shadow effect
            workbook.Save("CheckBoxWithShadow.xlsx");
            
            checkBox.Shadow = false; // Disable shadow effect
            workbook.Save("CheckBoxWithoutShadow.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


