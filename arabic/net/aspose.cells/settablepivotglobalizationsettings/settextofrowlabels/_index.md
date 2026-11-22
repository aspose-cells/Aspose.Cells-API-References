---
title: "SettablePivotGlobalizationSettings.SetTextOfRowLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تعيين نص تسمية Row Labels في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/settextofrowlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfRowLabels method

يضبط نص تسمية "Row Labels" في PivotTable.

```csharp
public void SetTextOfRowLabels(string text)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | نص تسميات الصفوف |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للسياق
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // أنشئ إعدادات العولمة
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            SettablePivotGlobalizationSettings pivotSettings = new SettablePivotGlobalizationSettings();
            globalizationSettings.PivotSettings = pivotSettings;

            try
            {
                // تعيين نص مخصص لـ "Row Labels"
                pivotSettings.SetTextOfRowLabels("Custom Row Labels");

                // تحقق من التغيير
                string rowLabelsText = pivotSettings.GetTextOfRowLabels();
                Console.WriteLine($"Row Labels text after change: {rowLabelsText}");

                // تطبيق الإعدادات على دفتر العمل
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // احفظ المصنف
                workbook.Save("SetTextOfRowLabelsDemo.xlsx");
                Console.WriteLine("SetTextOfRowLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfRowLabels: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


