---
title: "GlobalizationSettings.GetProtectionNameOfPivotTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على اسم الحماية في PivotTable"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getprotectionnameofpivottable/
---
## GlobalizationSettings.GetProtectionNameOfPivotTable method

يحصل على اسم الحماية في PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetProtectionNameOfPivotTable()
```

### قيمة الإرجاع

اسم الحماية في PivotTable

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetTextOfProtectedName(string). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء إعدادات تعميم قياسية
            GlobalizationSettings standardSettings = new GlobalizationSettings();
            
            // إنشاء إعدادات تعميم مخصصة
            GlobalizationSettings customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // الحصول على اسم الحماية الافتراضي
                string defaultName = standardSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Default protection name: {defaultName}");

                // الحصول على اسم الحماية المخصص
                string customName = customSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Custom protection name: {customName}");

                // إنشاء جدول محوري لتوضيح تطبيق الإعدادات
                worksheet.Cells["A1"].Value = "Data";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;
                int pivotIndex = worksheet.PivotTables.Add("A1", "A1:A4", "PivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // عادةً ما يتم تطبيق الحماية هنا باستخدام الاسم المسترجع
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetProtectionNameOfPivotTable: {ex.Message}");
            }
            
            workbook.Save("GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public new string GetProtectionNameOfPivotTable()
        {
            return "CustomPivotProtection";
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


