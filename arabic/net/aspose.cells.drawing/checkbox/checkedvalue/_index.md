---
title: "CheckBox.CheckedValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CheckBox. تحصل أو تضبط قيمة مربع الاختيار"
type: docs
url: /ar/net/aspose.cells.drawing/checkbox/checkedvalue/
---
## CheckBox.CheckedValue property

الحصول على أو تعيين قيمة خانة الاختيار.

```csharp
public CheckValueType CheckedValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyCheckedValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة خانة اختيار إلى ورقة العمل
            CheckBox checkBox = sheet.Shapes.AddCheckBox(1, 1, 100, 100, 20, 20);

            // عيّن قيمة مربع الاختيار إلى محدد
            checkBox.CheckedValue = CheckValueType.Checked;

            // احفظ المصنف
            workbook.Save("CheckBoxCheckedValueDemo.xlsx");

            // قم بتحميل المصنف المحفوظ للتحقق
            Workbook loadedWorkbook = new Workbook("CheckBoxCheckedValueDemo.xlsx");
            CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // إخراج حالة مربع الاختيار
            Console.WriteLine("CheckBox CheckedValue: " + loadedCheckBox.CheckedValue);
        }
    }
}
```

### انظر أيضًا

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


