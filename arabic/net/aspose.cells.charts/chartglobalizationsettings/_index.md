---
title: "الفئة ChartGlobalizationSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.ChartGlobalizationSettings الفئة. يمثل إعدادات العولمة لمخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartglobalizationsettings/
---
## ChartGlobalizationSettings class

يمثل إعدادات العولمة للمخطط.

```csharp
public class ChartGlobalizationSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ChartGlobalizationSettings](chartglobalizationsettings/)() | البناء الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [GetAxisTitleName](../../aspose.cells.charts/chartglobalizationsettings/getaxistitlename/)() | يحصل على اسم العنوان للمحور. |
| virtual [GetAxisUnitName](../../aspose.cells.charts/chartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | يحصل على اسم وحدة المحور. |
| virtual [GetChartTitleName](../../aspose.cells.charts/chartglobalizationsettings/getcharttitlename/)() | يحصل على اسم عنوان المخطط. |
| virtual [GetLegendDecreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/)() | يحصل على اسم الانخفاض للوسيلة الإيضاحية. |
| virtual [GetLegendIncreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/)() | يحصل على اسم الزيادة للوسيلة الإيضاحية. |
| virtual [GetLegendTotalName](../../aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/)() | يحصل على اسم الإجمالي للوسيلة الإيضاحية. |
| virtual [GetOtherName](../../aspose.cells.charts/chartglobalizationsettings/getothername/)() | يحصل على اسم تسميات "Other" للمخطط. |
| virtual [GetSeriesName](../../aspose.cells.charts/chartglobalizationsettings/getseriesname/)() | يحصل على اسم السلسلة في المخطط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartGlobalizationSettingsDemo
    {
        public static void ChartGlobalizationSettingsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مخططًا تجريبيًا إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // أنشئ نسخة من ChartGlobalizationSettings
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();

            // أظهر استخدام الأساليب في ChartGlobalizationSettings
            string seriesName = globalizationSettings.GetSeriesName();
            string chartTitleName = globalizationSettings.GetChartTitleName();
            string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();
            string legendTotalName = globalizationSettings.GetLegendTotalName();
            string axisTitleName = globalizationSettings.GetAxisTitleName();
            string otherName = globalizationSettings.GetOtherName();
            string axisUnitName = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);

            // اطبع الأسماء المسترجعة إلى وحدة التحكم
            Console.WriteLine("Series Name: " + seriesName);
            Console.WriteLine("Chart Title Name: " + chartTitleName);
            Console.WriteLine("Legend Increase Name: " + legendIncreaseName);
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);
            Console.WriteLine("Legend Total Name: " + legendTotalName);
            Console.WriteLine("Axis Title Name: " + axisTitleName);
            Console.WriteLine("Other Name: " + otherName);
            Console.WriteLine("Axis Unit Name: " + axisUnitName);

            // احفظ المصنف
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
            workbook.Save("ChartGlobalizationSettingsExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


