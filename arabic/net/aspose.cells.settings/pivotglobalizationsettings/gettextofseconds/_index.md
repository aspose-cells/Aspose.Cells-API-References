---
title: "PivotGlobalizationSettings.GetTextOfSeconds"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على النص المحلي للثواني"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/
---
## PivotGlobalizationSettings.GetTextOfSeconds method

يحصل على النص المحلي لـ "Seconds"

```csharp
public virtual string GetTextOfSeconds()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfSecondsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B2", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقل التاريخ إلى منطقة الصفوف
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // أنشئ إعدادات العولمة
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // عرض طريقة GetTextOfSeconds
            Console.WriteLine("Localized text for seconds: " + globalizationSettings.GetTextOfSeconds());

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


