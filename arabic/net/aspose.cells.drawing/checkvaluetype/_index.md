---
title: "التعداد CheckValueType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.CheckValueType. يمثل نوع قيمة التحقق لمربع الاختيار"
type: docs
url: /ar/net/aspose.cells.drawing/checkvaluetype/
---
## CheckValueType enumeration

يمثل نوع قيمة التحقق لمربع الاختيار.

```csharp
public enum CheckValueType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| UnChecked | `0` | غير محدد |
| Checked | `1` | محدد |
| Mixed | `2` | مختلط |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassCheckValueTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف مربعات اختيار إلى ورقة العمل
            int checkboxIndex1 = sheet.CheckBoxes.Add(0, 0, 100, 100);
            int checkboxIndex2 = sheet.CheckBoxes.Add(0, 1, 100, 100);

            // احصل على مربعات الاختيار واضبط خصائصها
            Aspose.Cells.Drawing.CheckBox checkbox1 = sheet.CheckBoxes[checkboxIndex1];
            Aspose.Cells.Drawing.CheckBox checkbox2 = sheet.CheckBoxes[checkboxIndex2];

            // تعيين قيم مربعات الاختيار وحالة التحديد
            checkbox1.Value = true;
            checkbox1.CheckedValue = CheckValueType.Checked;
            
            checkbox2.Value = false;
            checkbox2.CheckedValue = CheckValueType.UnChecked;  // Note: Changed from Unchecked to UnChecked

            // ربط مربعات الاختيار بالخلايا
            checkbox1.LinkedCell = "A1";
            checkbox2.LinkedCell = "A2";

            // إخراج قيم الخلايا لتوضيح الارتباط
            Console.WriteLine("Cell A1 value (should be true): " + sheet.Cells["A1"].BoolValue);
            Console.WriteLine("Cell A2 value (should be false): " + sheet.Cells["A2"].BoolValue);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


