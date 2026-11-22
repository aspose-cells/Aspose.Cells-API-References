---
title: "PivotTable.ShowDrill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. يحصل ويضبط ما إذا كان يتم عرض أزرار التوسيع/الطي"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showdrill/
---
## PivotTable.ShowDrill property

يحصل ويضبط ما إذا كان يتم عرض أزرار التوسيع/الطي.

```csharp
public bool ShowDrill { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDrillDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل وتعبئتها ببيانات عينة
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "Pivot";
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B4"].Value = 150;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // تمكين الحفر العمق وعرض مؤشرات الحفر
            pivotTable.EnableDrilldown = true;
            pivotTable.ShowDrill = true;
            
            // تحديث وحساب البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotTableShowDrillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


