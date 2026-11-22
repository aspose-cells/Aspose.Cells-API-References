---
title: "GlobalizationSettings.PivotSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GlobalizationSettings. تحصل أو تعين إعدادات العولمة لجدول المحور"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/pivotsettings/
---
## GlobalizationSettings.PivotSettings property

يحصل أو يحدد إعدادات العولمة لجدول المحور.

```csharp
public PivotGlobalizationSettings PivotSettings { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfTotal()
        {
            return "Custom Total";
        }

        public override string GetTextOfGrandTotal()
        {
            return "Custom Grand Total";
        }

        public override string GetTextOfDataFieldHeader()
        {
            return "DataCaption";
        }

        public override string GetTextOfProtectedName(string protectedName)
        {
            return protectedName + "2";
        }
    }

    public class GlobalizationSettingsPropertyPivotSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بيانات تجريبية
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Orange");
            dataSheet.Cells["B3"].PutValue(2000);

            // إنشاء جدول محوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int index = pivotSheet.PivotTables.Add("A1", "A1:B3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];
            
            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // تعيين إعدادات عولمة مخصصة لجدول المحور
            CustomPivotGlobalizationSettings pivotSettings = new CustomPivotGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings.PivotSettings = pivotSettings;

            // تحديث جدول المحور لتطبيق الإعدادات
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotGlobalizationSettings](../../../aspose.cells.settings/pivotglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


