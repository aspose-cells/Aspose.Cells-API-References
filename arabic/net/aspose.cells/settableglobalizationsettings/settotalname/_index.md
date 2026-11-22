---
title: "SettableGlobalizationSettings.SetTotalName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تعيين الاسم الكلي لدالة محددة"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/settotalname/
---
## SettableGlobalizationSettings.SetTotalName method

يضبط الاسم الكلي للدالة المحددة.

```csharp
public void SetTotalName(ConsolidationFunction functionType, string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| functionType | ConsolidationFunction | نوع الدالة. |
| name | String | الاسم الكلي للدالة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة للتجميع
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // تعيين اسم كلي مخصص لدالة Sum
                settings.SetTotalName(ConsolidationFunction.Sum, "Custom Sum Total");
                
                // تعيين اسم إجمالي مخصص لدالة Average
                settings.SetTotalName(ConsolidationFunction.Average, "Custom Average Total");

                // تطبيق الإعدادات على دفتر العمل
                workbook.Settings.GlobalizationSettings = settings;

                // تحقق من الإعدادات عن طريق استرجاع القيم
                string sumTotalName = settings.GetTotalName(ConsolidationFunction.Sum);
                string avgTotalName = settings.GetTotalName(ConsolidationFunction.Average);

                Console.WriteLine($"Sum total name set to: {sumTotalName}");
                Console.WriteLine($"Average total name set to: {avgTotalName}");

                // إنشاء جدول محوري لتوضيح التأثير
                worksheet.Cells["D1"].PutValue("Pivot Table");
                var pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
                var pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // احفظ المصنف
                workbook.Save("SetTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTotalName method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


