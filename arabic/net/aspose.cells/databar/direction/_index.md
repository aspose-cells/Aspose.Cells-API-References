---
title: "DataBar.Direction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataBar. يحصل أو يعيّن الاتجاه الذي يُعرض به شريط البيانات"
type: docs
url: /ar/net/aspose.cells/databar/direction/
---
## DataBar.Direction property

يحصل أو يضبط الاتجاه الذي يُعرض به شريط البيانات.

```csharp
public TextDirectionType Direction { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarPropertyDirectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لتوضيح أشرطة البيانات
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;  // Values from 1 to 10 in column A
            }

            // إضافة تنسيق شرطي لشريط البيانات
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection conditionalFormatting = conditionalFormattings[index];
            
            // حدد نطاق الخلية لشرط التنسيق
            CellArea cellArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 9,
                EndColumn = 0
            };
            conditionalFormatting.AddArea(cellArea);

            // أضف شرط شريط البيانات واحصل على المرجع
            int conditionIndex = conditionalFormatting.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditionalFormatting[conditionIndex];

            DataBar dataBar = condition.DataBar;

            // اعرض قيمة الاتجاه الحالية
            Console.WriteLine("Initial DataBar Direction: " + dataBar.Direction);

            // غيّر الاتجاه إلى من اليمين إلى اليسار ووضح ذلك
            dataBar.Direction = TextDirectionType.RightToLeft;

            // إعداد إضافي لتحسين التصور
            dataBar.Color = System.Drawing.Color.LightGreen;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;

            // احفظ المصنف لإظهار التأثير
            workbook.Save("DataBarDirectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextDirectionType](../../textdirectiontype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


