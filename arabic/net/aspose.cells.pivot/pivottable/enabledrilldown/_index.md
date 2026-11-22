---
title: "PivotTable.EnableDrilldown"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان التفصيل (drilldown) مفعلاً"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/enabledrilldown/
---
## PivotTable.EnableDrilldown property

يشير إلى ما إذا كان التفصيل (drilldown) مفعلاً.

```csharp
public bool EnableDrilldown { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableDrilldownDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل وتعبئتها ببيانات عينة
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // تكوين حقول الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // تمكين وظيفة التفصيل
            pivotTable.EnableDrilldown = true;
            
            // احفظ المصنف
            workbook.Save("PivotTableEnableDrilldownDemo.xlsx");
            
            // تحقق من أنه تم ضبط الخاصية
            Console.WriteLine("EnableDrilldown property is set to: " + pivotTable.EnableDrilldown);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


