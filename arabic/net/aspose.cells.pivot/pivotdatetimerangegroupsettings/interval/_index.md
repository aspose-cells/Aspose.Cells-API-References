---
title: "PivotDateTimeRangeGroupSettings.Interval"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotDateTimeRangeGroupSettings. تحصل على القيمة الداخلية للمجموعة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

يحصل على القيمة الداخلية للمجموعة.

```csharp
public double Interval { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyIntervalDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل ببيانات عينة
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // أضف بيانات تاريخية عينة
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
            dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
            dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
            dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
            dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
            dataSheet.Cells["A7"].PutValue(DateTime.Now);

            // أضف ورقة عمل جدول pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            
            // إضافة جدول محوري
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:A7", 
                "A1", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // إضافة حقل التاريخ إلى منطقة الصفوف
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateField = pivotTable.RowFields[0];

            // تجميع حسب الأيام مع فاصل قدره 2
            dateField.GroupBy(1, false);
            PivotDateTimeRangeGroupSettings groupSettings = 
                (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            
            // نظرًا لأن Interval للقراءة فقط، نحتاج إلى تعيينه أثناء التجميع
            // الفاصل يتم تعيينه فعليًا في معلمات طريقة GroupBy
            // هنا نتحقق فقط من قيمة الفاصل الزمني
            Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");

            // احفظ المصنف
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


