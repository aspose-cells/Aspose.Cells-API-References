---
title: "Enum PivotFieldGroupType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.PivotFieldGroupType enum. يمثل نوع المجموعة لحقل المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldgrouptype/
---
## PivotFieldGroupType enumeration

يمثل نوع المجموعة لحقل pivot.

```csharp
public enum PivotFieldGroupType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون مجموعة |
| DateTimeRange | `1` | مجمّع حسب نطاق DateTime. |
| NumbericRange | `2` | مجمّع حسب نطاق رقمي. |
| NumericRange | `2` | مجمّع حسب نطاق رقمي. |
| Discrete | `3` | مجمّع حسب نقاط منفصلة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotFieldGroupTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14; // m/d/yyyy format
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

            // تجميع حقل التاريخ
            PivotField dateField = pivotTable.RowFields[0];
            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // الوصول إلى إعدادات المجموعة وعرضها
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // احفظ المصنف
            workbook.Save("PivotFieldGroupTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


