---
title: "SettableGlobalizationSettings.SetTableRowTypeOfData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحدد اسم نوع صفوف الجدول التي تتكون من منطقة البيانات للجدول المشار إليه"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/settablerowtypeofdata/
---
## SettableGlobalizationSettings.SetTableRowTypeOfData method

يضبط اسم النوع لصفوف الجدول التي تتكون من منطقة البيانات للجدول المشار إليه.

```csharp
public void SetTableRowTypeOfData(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfDataWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء جدول
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

            // أنشئ إعدادات العولمة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // حدد اسمًا مخصصًا لصفوف البيانات في الجدول
                settings.SetTableRowTypeOfData("MyDataRegion");
                
                // تطبيق الإعدادات على دفتر العمل
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table row type of data set to: MyDataRegion");
                Console.WriteLine("In formulas, '#MyDataRegion' will now represent the data region instead of '#Data'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfData method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("SetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


