---
title: "PivotItem.IsDetailHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotItem. تحصل وتضبط ما إذا كانت تفاصيل هذا العنصر المخفي مخفية"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/isdetailhidden/
---
## PivotItem.IsDetailHidden property

يحصل ويضبط ما إذا كان تفصيل هذا العنصر المحوري مخفيًا.

```csharp
public bool IsDetailHidden { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsDetailHiddenDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["B5"].PutValue("Potato");
            sheet.Cells["C1"].PutValue("Amount");
            sheet.Cells["C2"].PutValue(10);
            sheet.Cells["C3"].PutValue(15);
            sheet.Cells["C4"].PutValue(20);
            sheet.Cells["C5"].PutValue(25);

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة حقول الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            
            // تحديث وحساب البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // إخفاء التفاصيل لفئة "Fruit"
            pivotTable.RowFields[0].PivotItems["Fruit"].IsDetailHidden = true;
            
            // احفظ المصنف
            wb.Save("PivotItemIsDetailHiddenDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


