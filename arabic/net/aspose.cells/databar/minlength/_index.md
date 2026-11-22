---
title: "DataBar.MinLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataBar. تمثل الحد الأدنى لطول شريط البيانات"
type: docs
url: /ar/net/aspose.cells/databar/minlength/
---
## DataBar.MinLength property

يمثل الحد الأدنى لطول شريط البيانات.

```csharp
public int MinLength { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(25);
            worksheet.Cells["A4"].PutValue(35);

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // إضافة شريط بيانات
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            DataBar dataBar = fc.DataBar;

            // تكوين شريط البيانات
            dataBar.Color = Color.Green;
            dataBar.MinLength = 10;  // Minimum length set to 10%
            dataBar.MaxLength = 100;

            workbook.Save("DataBarMinLengthDemo.xlsx");
            Console.WriteLine("DataBar with MinLength demo executed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


