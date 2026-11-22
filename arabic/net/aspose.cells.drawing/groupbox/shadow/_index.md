---
title: "GroupBox.Shadow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GroupBox. تشير إلى ما إذا كان الـ groupbox يحتوي على ظل"
type: docs
url: /ar/net/aspose.cells.drawing/groupbox/shadow/
---
## GroupBox.Shadow property

يشير إلى ما إذا كان مجموعة المربعات لها ظل.

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
    public class GroupBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف مربع مجموعة مع ظل
            GroupBox groupBoxWithShadow = worksheet.Shapes.AddGroupBox(1, 0, 1, 0, 200, 150);
            groupBoxWithShadow.Shadow = true;
            groupBoxWithShadow.Text = "GroupBox with Shadow";
            
            // أضف مربع مجموعة بدون ظل
            GroupBox groupBoxWithoutShadow = worksheet.Shapes.AddGroupBox(1, 2, 1, 0, 200, 150);
            groupBoxWithoutShadow.Shadow = false;
            groupBoxWithoutShadow.Text = "GroupBox without Shadow";
            
            // أضف أزرار راديو داخل مربعات المجموعة لتوضيح التجميع
            RadioButton radio1 = worksheet.Shapes.AddRadioButton(3, 0, 2, 0, 30, 100);
            radio1.Text = "Option 1";
            radio1.LinkedCell = "A1";
            
            RadioButton radio2 = worksheet.Shapes.AddRadioButton(6, 0, 2, 0, 30, 100);
            radio2.Text = "Option 2";
            radio2.LinkedCell = "A1";
            
            // اجمع الأشكال
            Shape[] shapes = { groupBoxWithShadow, radio1, radio2 };
            worksheet.Shapes.Group(shapes);
            
            // احفظ المصنف
            workbook.Save("GroupBoxShadowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GroupBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


