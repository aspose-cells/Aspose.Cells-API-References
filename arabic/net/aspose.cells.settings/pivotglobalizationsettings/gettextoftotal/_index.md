---
title: "PivotGlobalizationSettings.GetTextOfTotal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على نص تسمية Total في PivotTable. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي PivotTable على حقلين PivotFields أو أكثر في منطقة البيانات"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/
---
## PivotGlobalizationSettings.GetTextOfTotal method

يحصل على نص تسمية "Total" في PivotTable. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي PivotTable على حقلين PivotFields أو أكثر في منطقة البيانات.

```csharp
public virtual string GetTextOfTotal()
```

### قيمة الإرجاع

نص تسمية "Total"

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إنشاء واستخدام إعدادات العولمة
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // عرض طريقة GetTextOfTotal
            Console.WriteLine("Total label text: " + globalizationSettings.GetTextOfTotal());

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


