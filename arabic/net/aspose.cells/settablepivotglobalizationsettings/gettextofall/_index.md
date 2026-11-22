---
title: "SettablePivotGlobalizationSettings.GetTextOfAll"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تحصل على نص تسمية All في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/gettextofall/
---
## SettablePivotGlobalizationSettings.GetTextOfAll method

يحصل على نص التسمية "(All)" في جدول المحور.

```csharp
public override string GetTextOfAll()
```

### قيمة الإرجاع

نص تسمية "(All)"

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfAllDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(15);

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // أنشئ إعدادات العولمة
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();
            settings.SetTextOfAll("(All Items)");

            try
            {
                // احصل على النص الحالي لتسمية "(All)"
                string currentText = settings.GetTextOfAll();
                Console.WriteLine($"Current text of '(All)' label: {currentText}");

                // تحديث جدول Pivot بالإعدادات الجديدة
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfAll method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("MethodGetTextOfAllDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


