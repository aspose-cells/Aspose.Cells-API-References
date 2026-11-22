---
title: "DataBar.MaxCfvo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataBar. الحصول أو تعيين كائن القيمة القصوى لهذا الشريط. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Min إليه"
type: docs
url: /ar/net/aspose.cells/databar/maxcfvo/
---
## DataBar.MaxCfvo property

احصل أو اضبط كائن القيمة القصوى لهذا شريط البيانات. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Min إليه.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxCfvoDemo
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

            // إضافة تنسيق شرطي لشريط البيانات
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // إضافة شريط بيانات
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;

            // تعيين قيمة MaxCfvo
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            dataBar.MaxCfvo.Value = 50;

            // احفظ المصنف
            workbook.Save("DataBarMaxCfvoDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


