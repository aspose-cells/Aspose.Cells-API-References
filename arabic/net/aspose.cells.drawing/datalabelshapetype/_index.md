---
title: "تعداد DataLabelShapeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.DataLabelShapeType. يحدد هندسة الشكل المسبق التي ستُستخدم في المخطط"
type: docs
url: /ar/net/aspose.cells.drawing/datalabelshapetype/
---
## DataLabelShapeType enumeration

يحدد هندسة الشكل المسبقة التي ستُستخدم لمخطط.

```csharp
public enum DataLabelShapeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Rect | `0` | يمثل الشكل المستطيل. |
| RoundRect | `1` | يمثل شكل المستطيل المستدير. |
| Ellipse | `2` | يمثل شكل القطع الناقص. |
| RightArrowCallout | `3` | يمثل شكل الفقاعة ذات السهم الأيمن. |
| DownArrowCallout | `4` | يمثل شكل الفقاعة ذات السهم السفلي. |
| LeftArrowCallout | `5` | يمثل شكل الفقاعة ذات السهم الأيسر. |
| UpArrowCallout | `6` | يمثل شكل الفقاعة ذات السهم العلوي. |
| WedgeRectCallout | `7` | يمثل شكل الفقاعة ذات المستطيل القطاعي. |
| WedgeRoundRectCallout | `8` | يمثل شكل الفقاعة ذات المستطيل المستدير القطاعي. |
| WedgeEllipseCallout | `9` | يمثل شكل الفقاعة ذات القطع الناقص القطاعي. |
| LineCallout | `10` | يمثل شكل الفقاعة ذات الخط. |
| BentLineCallout | `11` | يمثل شكل الفقاعة ذات الخط المنحني. |
| LineWithAccentBarCallout | `12` | يمثل شكل الفقاعة ذات الخط مع شريط التمييز. |
| BentLineWithAccentBarCallout | `13` | يمثل شكل الفقاعة ذات الخط المنحني مع شريط التمييز. |
| Line | `14` | هذا النوع يُستخدم فقط لمعالجة الملفات الخاصة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class DataLabelShapeTypeDemo
    {
        public static void DataLabelShapeTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى السلسلة الأولى في المخطط
            Series series = chart.NSeries[0];

            // تمكين تسميات البيانات للسلسلة
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // احفظ المصنف
            workbook.Save("DataLabelShapeTypeExample.xlsx");
            workbook.Save("DataLabelShapeTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


