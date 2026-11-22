---
title: "ColorScale.MinColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ColorScale. الحصول على أو تعيين لون التدرج للقيمة الدنيا في النطاق"
type: docs
url: /ar/net/aspose.cells/colorscale/mincolor/
---
## ColorScale.MinColor property

احصل أو عيّن لون التدرج للقيمة الدنيا في النطاق.

```csharp
public Color MinColor { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinColorDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
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
            
            // إنشاء كائن CellArea بدلاً من استخدام سلسلة
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // تهيئة مقياس اللون
            ColorScale colorScale = fc.ColorScale;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // تعيين أنواع القيم
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            colorScale.MidCfvo.Value = 50;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // احفظ المصنف
            workbook.Save("ColorScaleMinColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


