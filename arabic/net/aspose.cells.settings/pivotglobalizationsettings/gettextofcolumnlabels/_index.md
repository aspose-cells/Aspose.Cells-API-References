---
title: "PivotGlobalizationSettings.GetTextOfColumnLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على نص تسمية Column Labels في PivotTable"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextofcolumnlabels/
---
## PivotGlobalizationSettings.GetTextOfColumnLabels method

يحصل على نص التسمية "Column Labels" في جدول المحور.

```csharp
public virtual string GetTextOfColumnLabels()
```

### قيمة الإرجاع

نص تسميات الأعمدة

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(800);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إنشاء واستخدام إعدادات العولمة
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // عرض GetTextOfColumnLabels
            Console.WriteLine("Column Labels Text: " + globalizationSettings.GetTextOfColumnLabels());

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


