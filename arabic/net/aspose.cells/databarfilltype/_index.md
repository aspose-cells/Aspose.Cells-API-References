---
title: "تعداد DataBarFillType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.DataBarFillType. يحدد كيفية تعبئة شريط البيانات باللون"
type: docs
url: /ar/net/aspose.cells/databarfilltype/
---
## DataBarFillType enumeration

يحدد كيفية تعبئة شريط البيانات باللون.

```csharp
public enum DataBarFillType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Solid | `0` | يتم تعبئة شريط البيانات بلون صلب. |
| Gradient | `1` | يتم تعبئة شريط البيانات بتدرج لوني. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarFillTypeDemo
    {
        public static void DataBarFillTypeExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet sheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // يحدد نطاق التنسيق الشرطي.
            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // يضيف شرطًا
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // الحصول على Databar
            DataBar dataBar = cond.DataBar;

            // تعيين خصائص Databar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // ضع قيم الخلايا
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // حفظ ملف Excel
            workbook.Save("DataBarFillTypeExample.xlsx");
            workbook.Save("DataBarFillTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


