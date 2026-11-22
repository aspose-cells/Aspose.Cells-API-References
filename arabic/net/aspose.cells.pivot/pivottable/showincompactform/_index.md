---
title: "PivotTable.ShowInCompactForm"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تنسيق عرض PivotTable في الشكل المدمج"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showincompactform/
---
## PivotTable.ShowInCompactForm method

يصمم عرض PivotTable في شكل مدمج.

```csharp
public void ShowInCompactForm()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInCompactFormDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل من بيانات المصدر
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Product");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Electronics");
            sourceSheet.Cells["B2"].PutValue("Laptop");
            sourceSheet.Cells["C2"].PutValue(1200);
            
            sourceSheet.Cells["A3"].PutValue("Electronics");
            sourceSheet.Cells["B3"].PutValue("Phone");
            sourceSheet.Cells["C3"].PutValue(800);
            
            sourceSheet.Cells["A4"].PutValue("Furniture");
            sourceSheet.Cells["B4"].PutValue("Chair");
            sourceSheet.Cells["C4"].PutValue(150);
            
            sourceSheet.Cells["A5"].PutValue("Furniture");
            sourceSheet.Cells["B5"].PutValue("Table");
            sourceSheet.Cells["C5"].PutValue(300);

            // إنشاء ورقة عمل جدول محوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // إضافة جدول محوري
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("=Sheet1!A1:C5", "A3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // إضافة حقول إلى المناطق
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // تعيين جدول المحوري لعرضه في الشكل المدمج
            pivotTable.ShowInCompactForm();
            
            // حساب البيانات وتحديثها
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // احفظ المصنف
            workbook.Save("PivotTableCompactFormDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


