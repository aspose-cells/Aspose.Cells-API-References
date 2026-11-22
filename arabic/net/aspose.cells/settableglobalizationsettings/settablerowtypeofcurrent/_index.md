---
title: "SettableGlobalizationSettings.SetTableRowTypeOfCurrent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحدد اسم النوع لصفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/
---
## SettableGlobalizationSettings.SetTableRowTypeOfCurrent method

يضبط اسم النوع لصفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه.

```csharp
public void SetTableRowTypeOfCurrent(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfCurrentWithStringDemo
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
            cells["B2"].PutValue("2.5");
            cells["A3"].PutValue("Banana");
            cells["B3"].PutValue("1.5");
            
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // أنشئ إعدادات العولمة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // تعيين اسم مخصص لنوع الصف الحالي
                settings.SetTableRowTypeOfCurrent("CurrentItem");
                
                // تطبيق الإعدادات على دفتر العمل
                workbook.Settings.GlobalizationSettings = settings;

                // تحقق من الإعداد عن طريق استرجاع القيمة
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine($"Current row type name set to: {currentRowType}");

                // احفظ المصنف
                workbook.Save("SetTableRowTypeOfCurrentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfCurrent method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


