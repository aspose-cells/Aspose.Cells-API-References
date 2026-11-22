---
title: "PivotDateTimeRangeGroupSettings.GroupByTypes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotDateTimeRangeGroupSettings. تحصل على أنواع التجميع حسب التاريخ والوقت"
type: docs
url: /ar/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/
---
## PivotDateTimeRangeGroupSettings.GroupByTypes property

يحصل على أنواع التجميع حسب التاريخ والوقت.

```csharp
public PivotGroupByType[] GroupByTypes { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDateTimeRangeGroupSettingsPropertyGroupByTypesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة مع تواريخ
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // إنشاء جدول محوري
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // إضافة حقول إلى جدول محوري
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // تجميع حسب التاريخ مع أنواع تجميع متعددة
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                PivotGroupByType[] groupTypes = new PivotGroupByType[]
                {
                    PivotGroupByType.Months,
                    PivotGroupByType.Quarters
                };
                dateField.GroupBy(startDate, endDate, groupTypes, 1, false);

                // الوصول إلى إعدادات المجموعة وإظهار خاصية GroupByTypes
                PivotDateTimeRangeGroupSettings groupSettings =
                    (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // اعرض قيمة خاصية GroupByTypes
                Console.WriteLine("GroupByTypes values:");
                foreach (PivotGroupByType type in groupSettings.GroupByTypes)
                {
                    Console.WriteLine(type);
                }

                // حفظ النتيجة
                workbook.Save("GroupByTypesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


