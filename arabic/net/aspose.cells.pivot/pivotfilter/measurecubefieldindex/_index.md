---
title: "PivotFilter.MeasureCubeFieldIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFilter. تحدد فهرس حقل مكعب القياس. تُستخدم هذه الخاصية فقط بواسطة المرشحات في محاور OLAP وتحدد على أي قياس يجب تطبيق مرشح القيمة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/measurecubefieldindex/
---
## PivotFilter.MeasureCubeFieldIndex property

يحدد فهرس حقل مكعب القياس. تُستخدم هذه الخاصية فقط بواسطة المرشحات في جداول المحور OLAP وتحدد على أي قياس يجب أن يُطبق مرشح القيمة.

```csharp
public int MeasureCubeFieldIndex { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMeasureCubeFieldIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل وتعبئتها ببيانات عينة
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة صفوف وحقول بيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // تحديث بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // إضافة مرشح إلى جدول pivot
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.BaseFields[0];
            
            // إنشاء وإضافة مرشح عبر PivotTable بدلاً من PivotField
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            
            // عرض MeasureCubeFieldIndex
            Console.WriteLine("MeasureCubeFieldIndex: " + filter.MeasureCubeFieldIndex);
            
            // احفظ المصنف
            workbook.Save("PivotFilterMeasureCubeFieldIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


