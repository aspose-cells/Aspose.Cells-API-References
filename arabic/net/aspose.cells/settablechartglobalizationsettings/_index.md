---
title: "الفئة SettableChartGlobalizationSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.SettableChartGlobalizationSettings. تنفيذ PivotGlobalizationSettings الذي يدعم المستخدم لتعيين/تغيير النصوص المحددة مسبقًا"
type: docs
url: /ar/net/aspose.cells/settablechartglobalizationsettings/
---
## SettableChartGlobalizationSettings class

تنفيذ PivotGlobalizationSettings الذي يدعم المستخدم في تعيين/تغيير النصوص المحددة مسبقًا.

```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | البناء الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | يحصل على اسم العنوان للمحور. |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | يحصل على اسم وحدة المحور. |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | يحصل على اسم عنوان المخطط. |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | يحصل على اسم الانخفاض للوسيلة الإيضاحية. |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | يحصل على اسم الزيادة للوسيلة الإيضاحية. |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | يحصل على اسم الإجمالي للوسيلة الإيضاحية. |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | يحصل على اسم تسميات "Other" للمخطط. |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | يحصل على اسم السلسلة في المخطط. |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | يضبط اسم العنوان للمحور. |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | يضبط اسم وحدة المحور. |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | يضبط اسم عنوان المخطط. |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | يضبط اسم الانخفاض للوسيلة الإيضاحية. |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | يضبط اسم الزيادة للوسيلة الإيضاحية. |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | يضبط اسم الإجمالي للوسيلة الإيضاحية. |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | يضبط اسم تسميات "Other" للمخطط. |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | يضبط اسم السلسلة في المخطط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CellsClassSettableChartGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء نسخة من SettableChartGlobalizationSettings
                var settings = new SettableChartGlobalizationSettings();

                // تعيين إعدادات العولمة المخصصة
                settings.SetSeriesName("Custom Series");
                settings.SetChartTitleName("Custom Chart Title");
                settings.SetLegendIncreaseName("Custom Increase");
                settings.SetLegendDecreaseName("Custom Decrease");

                // إنشاء تنفيذ مخصص لـ GlobalizationSettings
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);

                // إنشاء مخطط بسيط لعرض الإعدادات
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Q1");
                worksheet.Cells["A3"].PutValue("Q2");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);

                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";
                chart.Title.Text = "Demo Chart";

                Console.WriteLine("SettableChartGlobalizationSettings configured successfully");
                workbook.Save("SettableChartGlobalizationSettingsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SettableChartGlobalizationSettings: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            private readonly SettableChartGlobalizationSettings _chartSettings;

            public CustomGlobalizationSettings(SettableChartGlobalizationSettings chartSettings)
            {
                _chartSettings = chartSettings;
            }

            // تنفيذ طرق GlobalizationSettings المطلوبة هنا
            // التي تفوض إلى مثيل SettableChartGlobalizationSettings
        }
    }
}
```

### انظر أيضًا

* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


