---
title: "PivotTable.PageFieldWrapCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable."
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/pagefieldwrapcount/
---
## PivotTable.PageFieldWrapCount property

يحصل على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable.

```csharp
public int PageFieldWrapCount { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldWrapCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // أدخل البيانات
            Worksheet data = workbook.Worksheets.Add("data");
            data.Cells["A1"].PutValue("Country");
            data.Cells["B1"].PutValue("Product");
            data.Cells["C1"].PutValue("Vendor");
            data.Cells["D1"].PutValue("Value");
            data.Cells["A2"].PutValue("USA");
            data.Cells["B2"].PutValue("Car");
            data.Cells["C2"].PutValue("Ford");
            data.Cells["D2"].PutValue(1200.987654321);
            data.Cells["A3"].PutValue("Japan");
            data.Cells["B3"].PutValue("Bike");
            data.Cells["C3"].PutValue("Yamaha");
            data.Cells["D3"].PutValue(985.123456789);

            // إنشاء جدول محوري
            Worksheet pivot = workbook.Worksheets.Add("pivot");
            PivotTableCollection pivotTables = pivot.PivotTables;
            int index = pivotTables.Add("=data!A1:D3", "A1", "pivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // عيّن خاصية PageFieldWrapCount
            pivotTable.PageFieldWrapCount = 2; // Number of page fields per row
            
            // احسب وقم بتحديث جدول المحور
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotTablePageFieldWrapCountDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


