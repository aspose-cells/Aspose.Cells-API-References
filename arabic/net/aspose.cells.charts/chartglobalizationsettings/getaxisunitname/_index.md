---
title: "ChartGlobalizationSettings.GetAxisUnitName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartGlobalizationSettings. تحصل على اسم وحدة المحور"
type: docs
url: /ar/net/aspose.cells.charts/chartglobalizationsettings/getaxisunitname/
---
## ChartGlobalizationSettings.GetAxisUnitName method

يحصل على اسم وحدة المحور.

```csharp
public virtual string GetAxisUnitName(DisplayUnitType type)
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // إنشاء إعدادات العولمة والحصول على اسم وحدة المحور
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string thousandsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);
            string millionsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Millions);

            // إخراج النتائج
            Console.WriteLine("Thousands unit name: " + thousandsUnit);
            Console.WriteLine("Millions unit name: " + millionsUnit);

            // احفظ دفتر العمل
            workbook.Save("AxisUnitNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [DisplayUnitType](../../displayunittype/)
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


