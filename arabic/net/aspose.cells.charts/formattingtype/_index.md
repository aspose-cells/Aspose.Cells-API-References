---
title: "Enum FormattingType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.FormattingType enum. يمثل نوع التنسيق المطبق على كائن Area أو كائن Line"
type: docs
url: /ar/net/aspose.cells.charts/formattingtype/
---
## FormattingType enumeration

يمثل نوع التنسيق المطبق على كائن [`Area`](../../aspose.cells.drawing/area/) أو كائن [`Line`](../../aspose.cells.drawing/line/).

```csharp
public enum FormattingType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | يمثل نوع التنسيق التلقائي. |
| Custom | `2` | يمثل نوع تنسيق مخصص. |
| None | `1` | يمثل نوع التنسيق لا شيء. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class FormattingTypeDemo
    {
        public static void FormattingTypeExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى كائن Workbook
            int sheetIndex = workbook.Worksheets.Add();
            
            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // إضافة قيم عينة إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // ضبط لون المقدمة لمنطقة الرسم
            chart.PlotArea.Area.ForegroundColor = Color.Blue;
            chart.PlotArea.Area.Formatting = FormattingType.Custom;
            
            // ضبط لون المقدمة لمنطقة المخطط
            chart.ChartArea.Area.ForegroundColor = Color.Yellow;
            chart.ChartArea.Area.Formatting = FormattingType.Automatic;
            
            // ضبط لون المقدمة لمنطقة NSeries الأولى
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.Formatting = FormattingType.None;
            
            // ضبط لون المقدمة لمنطقة النقطة الأولى في NSeries
            chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
            chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
            
            // حفظ ملف Excel
            workbook.Save("FormattingTypeExample.xlsx");
            workbook.Save("FormattingTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


