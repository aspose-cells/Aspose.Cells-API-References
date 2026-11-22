---
title: "تعداد DataBarAxisPosition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.DataBarAxisPosition. يحدد موضع المحور لنطاق من الخلايا مع تنسيق شرطي كأشرطة بيانات"
type: docs
url: /ar/net/aspose.cells/databaraxisposition/
---
## DataBarAxisPosition enumeration

يحدد موضع المحور لنطاق من الخلايا ذات التنسيق الشرطي كأشرطة بيانات.

```csharp
public enum DataBarAxisPosition
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | عرض المحور في موضع متغيّر بناءً على نسبة القيمة السالبة الدنيا إلى القيمة الموجبة القصوى في النطاق. تُعرض القيم الموجبة من اليسار إلى اليمين. تُعرض القيم السالبة من اليمين إلى اليسار. عندما تكون جميع القيم موجبة أو جميعها سالبة، لا يتم عرض أي محور. |
| Midpoint | `1` | عرض المحور في منتصف الخلية بغض النظر عن مجموعة القيم في النطاق. تُعرض القيم الموجبة من اليسار إلى اليمين. تُعرض القيم السالبة من اليمين إلى اليسار. |
| None | `2` | لا يتم عرض أي محور، وتُعرض القيم الموجبة والسالبة معًا من اليسار إلى اليمين. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarAxisPositionDemo
    {
        public static void DataBarAxisPositionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى في المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة قاعدة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // تحديد نطاق التنسيق الشرطي
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);
            
            // إضافة شرط شريط بيانات
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];
            DataBar dataBar = fc.DataBar;
            
            // تحديد خصائص شريط البيانات
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint; // Using DataBarAxisPosition enum
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            
            // إدخال قيم الخلايا
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);
            
            // حفظ ملف Excel
            workbook.Save("DataBarAxisPositionExample.xlsx");
            workbook.Save("DataBarAxisPositionExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


