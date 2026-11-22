---
title: "PivotField.RegionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تحدد منطقة جدول المحور التي يُعرض فيها هذا الحقل"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/regiontype/
---
## PivotField.RegionType property

يحدد منطقة جدول المحور التي يُعرض فيها هذا الحقل.

```csharp
public PivotFieldType RegionType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyRegionTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تحديث بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احصل على حقل الـ pivot الأول
            PivotField pivotField = pivotTable.RowFields[0];

            // اعرض قيمة RegionType الحالية
            Console.WriteLine("Current RegionType value: " + pivotField.RegionType);

            // أظهر كيفية استخدام خاصية RegionType
            if (pivotField.RegionType == PivotFieldType.Row)
            {
                Console.WriteLine("This pivot field is in the row area");
            }

            // احفظ المصنف
            workbook.Save("PivotFieldRegionTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


