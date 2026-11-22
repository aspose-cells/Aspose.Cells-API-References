---
title: "التعداد PivotGroupByType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Pivot.PivotGroupByType. يمثل نوع التجميع."
type: docs
url: /ar/net/aspose.cells.pivot/pivotgroupbytype/
---
## PivotGroupByType enumeration

يمثل نوع التجميع حسب.

```csharp
[Flags]
public enum PivotGroupByType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| RangeOfValues | `1` | تجميع حسب الأرقام. |
| Numbers | `1` | تجميع حسب الأرقام. |
| Seconds | `2` | يعرض نوع التجميع للثواني. |
| Minutes | `4` | يعرض نوع التجميع للدقائق. |
| Hours | `8` | يعرض نوع التجميع للساعات. |
| Days | `10` | يعرض نوع التجميع للأيام. |
| Months | `20` | يعرض نوع التجميع للأشهر. |
| Quarters | `40` | يعرض نوع التجميع للربع. |
| Years | `80` | يعرض نوع التجميع للسنوات. |
| DateTimes | `FE` | يعرض جميع أنواع التجميع لتواريخ الوقت. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGroupByTypeDemo
    {
        public static void PivotGroupByTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14;//m/d/yyy
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].SetStyle(style);

            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].SetStyle(style);

            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A4"].SetStyle(style);

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field

            //TODO
            PivotField dateField = pivotTable.RowFields[0];

            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // الوصول إلى إعدادات المجموعة
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

            // إخراج إعدادات المجموعة
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Start Date: " + groupSettings.Start);
            Console.WriteLine("End Date: " + groupSettings.End);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // احفظ المصنف
            workbook.Save("PivotGroupByTypeExample.xlsx");
            
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


