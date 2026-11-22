---
title: "SettableGlobalizationSettings.SetTableRowTypeOfTotals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحدد اسم النوع لصفوف الجدول التي تتكون من صف الإجمالي للجدول المشار إليه"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/
---
## SettableGlobalizationSettings.SetTableRowTypeOfTotals method

يضبط اسم النوع لصفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه.

```csharp
public void SetTableRowTypeOfTotals(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم نوع صفوف الجدول |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfTotalsWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء جدول
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(10);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(15);
            cells["A4"].PutValue("Total");
            cells["B4"].PutValue("=SUM(B2:B3)");

            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;

            // أنشئ إعدادات العولمة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // استدعِ SetTableRowTypeOfTotals بالاسم المخصص
                settings.SetTableRowTypeOfTotals("CustomTotals");

                // تطبيق الإعدادات على دفتر العمل
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetTableRowTypeOfTotals executed successfully with parameter: CustomTotals");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfTotals method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("SetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


