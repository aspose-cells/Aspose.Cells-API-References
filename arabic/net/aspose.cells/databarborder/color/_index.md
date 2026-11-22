---
title: "DataBarBorder.Color"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataBarBorder. تحصل أو تعين لون حدود أشرطة البيانات المحددة بواسطة قاعدة تنسيق شرطي"
type: docs
url: /ar/net/aspose.cells/databarborder/color/
---
## DataBarBorder.Color property

يحصل أو يعيّن لون حد أشرطة البيانات المحددة بواسطة قاعدة تنسيق شرطي.

```csharp
public Color Color { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء مجموعة شرط تنسيق
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(new CellArea { StartRow = 2, StartColumn = 4, EndRow = 3, EndColumn = 6 });

            // إضافة شرط تنسيق شريط البيانات
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // تعيين خصائص شريط البيانات
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // تعيين خصائص الحدود (توضيح استخدام اللون)
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // احفظ المصنف
            workbook.Save("DataBarBorderColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar border color demo completed.");
        }
    }
}
```

### انظر أيضًا

* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


