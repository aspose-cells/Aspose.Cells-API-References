---
title: "PivotGlobalizationSettings.GetTextOfAllPeriods"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. يحصل على النص المترجم لجميع الفترات"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/
---
## PivotGlobalizationSettings.GetTextOfAllPeriods method

يحصل على النص المترجم لـ "All Periods".

```csharp
public virtual string GetTextOfAllPeriods()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOfAllPeriodsDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // إضافة بيانات عينة لإنشاء سياق لجدول المحور
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["B1"].PutValue("Sales");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["B2"].PutValue(1000);
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["B3"].PutValue(2000);
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B4"].PutValue(3000);

                // إنشاء جدول محوري
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // إنشاء مثال PivotGlobalizationSettings
                PivotGlobalizationSettings settings = new PivotGlobalizationSettings();

                // توضيح طريقة GetTextOfAllPeriods
                string allPeriodsText = settings.GetTextOfAllPeriods();
                Console.WriteLine("All Periods Text: " + allPeriodsText);

                // عرض تسميات الفترات الزمنية المرتبطة للسياق
                Console.WriteLine("Years Text: " + settings.GetTextOfYears());
                Console.WriteLine("Quarters Text: " + settings.GetTextOfQuarters());
                Console.WriteLine("Months Text: " + settings.GetTextOfMonths());

                // احفظ المصنف
                workbook.Save("GetTextOfAllPeriodsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


