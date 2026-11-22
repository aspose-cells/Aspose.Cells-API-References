---
title: "PivotTable.CalculateRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تحسب نطاق جداول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/calculaterange/
---
## PivotTable.CalculateRange method

يحسب نطاق جدول المحور.

```csharp
public void CalculateRange()
```

### ملاحظات

إذا لم يتم استدعاء هذه الطريقة، قد يكون نطاق جدول المحور غير مصحح.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بيانات نموذجية إلى الورقة الأولى
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Banana");
            dataSheet.Cells["B3"].PutValue(2000);
            dataSheet.Cells["A4"].PutValue("Orange");
            dataSheet.Cells["B4"].PutValue(3000);

            // إضافة جدول محوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("A1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // إضافة صفوف وحقول بيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // احسب النطاق وقم بتحديث البيانات
            pivotTable.CalculateRange();
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // احفظ المصنف
            workbook.Save("PivotTableCalculateRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


