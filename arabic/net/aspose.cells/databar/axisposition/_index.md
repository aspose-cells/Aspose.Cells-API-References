---
title: "DataBar.AxisPosition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataBar. يحصل أو يعيّن موضع محور أشرطة البيانات المحددة بقاعدة تنسيق شرطي"
type: docs
url: /ar/net/aspose.cells/databar/axisposition/
---
## DataBar.AxisPosition property

يحصل أو يضبط موضع محور أشرطة البيانات المحددة بواسطة قاعدة تنسيق شرطي.

```csharp
public DataBarAxisPosition AxisPosition { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyAxisPositionDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["E3"].PutValue(10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-15);
            sheet.Cells["G4"].PutValue(-25);

            // إضافة تنسيق شرطي لشريط البيانات
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];
            
            // تكوين خصائص شريط البيانات
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;
            
            // تعيين موضع المحور (عرض أساسي)
            cond.DataBar.AxisPosition = DataBarAxisPosition.Automatic;
            cond.DataBar.AxisColor = Color.Red;

            // احفظ المصنف
            workbook.Save("DataBarAxisPositionDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar with AxisPosition demo created successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [DataBarAxisPosition](../../databaraxisposition/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


