---
title: "PivotGlobalizationSettings.GetTextOfDays"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على النص المحلي للأيام"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextofdays/
---
## PivotGlobalizationSettings.GetTextOfDays method

يحصل على النص المحلي لـ "Days".

```csharp
public virtual string GetTextOfDays()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfDaysDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(1500);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقل التاريخ إلى منطقة الصفوف
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // أنشئ إعدادات العولمة
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // إظهار طريقة GetTextOfDays
            Console.WriteLine("Localized text for days: " + globalizationSettings.GetTextOfDays());

            // احفظ المصنف
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


