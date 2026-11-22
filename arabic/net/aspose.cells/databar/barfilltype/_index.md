---
title: "DataBar.BarFillType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataBar. تحصل أو تعين كيفية تعبئة شريط البيانات باللون"
type: docs
url: /ar/net/aspose.cells/databar/barfilltype/
---
## DataBar.BarFillType property

يحصل أو يضبط طريقة ملء شريط البيانات باللون.

```csharp
public DataBarFillType BarFillType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarFillTypeDemo
    {
        public static void Run()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // تحديد نطاق التنسيق الشرطي
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 5,
                StartColumn = 0,
                EndColumn = 5
            };
            fcs.AddArea(ca);

            // إضافة شرط DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // تكوين خصائص DataBar
            DataBar dataBar = fc.DataBar;
            dataBar.BarFillType = DataBarFillType.Gradient; // Demonstrating BarFillType usage
            dataBar.Color = Color.Blue;

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(100);

            // احفظ المصنف
            workbook.Save("DataBarFillTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [DataBarFillType](../../databarfilltype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


