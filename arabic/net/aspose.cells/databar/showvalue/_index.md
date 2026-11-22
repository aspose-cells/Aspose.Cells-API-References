---
title: "DataBar.ShowValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataBar. احصل أو عيّن العلامة التي تشير إلى ما إذا كان يجب إظهار قيم الخلايا التي يُطبق عليها هذا شريط البيانات. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/databar/showvalue/
---
## DataBar.ShowValue property

احصل أو اضبط العلامة التي تشير إلى ما إذا كان يجب إظهار قيم الخلايا التي يُطبق عليها شريط البيانات هذا. القيمة الافتراضية هي true.

```csharp
public bool ShowValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyShowValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // إضافة تنسيق شرطي لشريط البيانات
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // إضافة شرط شريط البيانات
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            
            // تعيين خصائص شريط البيانات
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.DataBar.Color = Color.Green;
            
            // عرض خاصية ShowValue
            fc.DataBar.ShowValue = true; // Show cell values along with data bars
            
            // احفظ المصنف
            workbook.Save("DataBarShowValueDemo.xlsx");
            
            Console.WriteLine("DataBar ShowValue demo completed. Output file: DataBarShowValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


