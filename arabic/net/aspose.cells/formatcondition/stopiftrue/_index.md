---
title: "FormatCondition.StopIfTrue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "FormatCondition property. True لا يمكن تطبيق أي قواعد ذات أولوية أقل على هذه القاعدة عندما تُقيم هذه القاعدة إلى true. ينطبق فقط على Excel 2007"
type: docs
url: /ar/net/aspose.cells/formatcondition/stopiftrue/
---
## FormatCondition.StopIfTrue property

صحيح، لا يمكن تطبيق أي قواعد ذات أولوية أقل فوق هذه القاعدة عندما تُقيم هذه القاعدة إلى true. ينطبق فقط على Excel 2007؛

```csharp
public bool StopIfTrue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStopIfTrueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // إضافة شرط وتعيين StopIfTrue
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            FormatCondition condition = fcs[conditionIndex];
            condition.StopIfTrue = true;
            
            // إضافة شرط آخر عادةً ما يتجاوز الأول
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "25", "");
            FormatCondition condition2 = fcs[conditionIndex2];
            condition2.StopIfTrue = false;

            // احفظ المصنف
            workbook.Save("StopIfTrueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


