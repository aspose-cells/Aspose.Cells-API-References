---
title: "DataBar.MaxLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataBar. تمثل الحد الأقصى لطول شريط البيانات"
type: docs
url: /ar/net/aspose.cells/databar/maxlength/
---
## DataBar.MaxLength property

يمثل الحد الأقصى لطول شريط البيانات.

```csharp
public int MaxLength { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // إضافة تنسيق شرطي
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            
            CellArea area = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(area);

            // إضافة شريط بيانات وتعيين الخصائص
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;
            
            dataBar.Color = Color.Blue;
            dataBar.MinLength = 0;
            dataBar.MaxLength = 90; // Demonstrating MaxLength property
            
            workbook.Save("DataBarMaxLengthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


