---
title: "DataBar.MinCfvo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataBar. احصل أو عيّن كائن قيمة الحد الأدنى لهذا DataBars. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Max إليه"
type: docs
url: /ar/net/aspose.cells/databar/mincfvo/
---
## DataBar.MinCfvo property

احصل أو اضبط كائن القيمة الدنيا لهذا شريط البيانات. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Max إليه.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinCfvoDemo
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

            // احصل على مجموعة التنسيق الشرطي
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];

            // إنشاء شريط بيانات مع تعيين MinCfvo إلى النوع \"Value\"
            fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[0].DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MinCfvo.Value = "5"; // Minimum value for the data bar

            // تعيين نطاق شريط البيانات
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // احفظ المصنف
            workbook.Save("DataBarMinCfvoDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


