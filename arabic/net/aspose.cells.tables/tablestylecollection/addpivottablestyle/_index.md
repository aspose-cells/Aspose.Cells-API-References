---
title: "TableStyleCollection.AddPivotTableStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TableStyleCollection. تضيف نمط جدول محوري مخصص"
type: docs
url: /ar/net/aspose.cells.tables/tablestylecollection/addpivottablestyle/
---
## TableStyleCollection.AddPivotTableStyle method

يضيف نمط جدول محوري مخصص.

```csharp
public int AddPivotTableStyle(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم نمط جدول المحور. |

### قيمة الإرجاع

فهرس نمط جدول المحور.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionMethodAddPivotTableStyleWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Desktop");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(500);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 1);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2);

            try
            {
                // احصل على مجموعة أنماط الجدول
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // استدعِ AddPivotTableStyle مع معامل من نوع String
                int styleIndex = tableStyles.AddPivotTableStyle("CustomPivotStyle1");
                Console.WriteLine($"Added pivot table style at index: {styleIndex}");

                // عيّن النمط الجديد كنمط محوري افتراضي
                tableStyles.DefaultPivotStyleName = "CustomPivotStyle1";

                // طبق النمط على جدولنا المحوري
                pivotTable.PivotTableStyleName = "CustomPivotStyle1";
                Console.WriteLine("Applied custom pivot table style successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPivotTableStyle method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("TableStyleCollectionMethodAddPivotTableStyleWithStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


