---
title: "PivotTable.SelectArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. حدد منطقة من عرض جدول المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/selectarea/
---
## PivotTable.SelectArea method

حدد منطقة من عرض جدول المحور.

```csharp
public PivotAreaCollection SelectArea(CellArea ca)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | منطقة الخلية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodSelectAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // حساب البيانات
            pivotTable.CalculateData();

            // حدد منطقة الخلية التي تريد اختيارها
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 5;
            area.EndColumn = 6;

            try
            {
                // استدعِ طريقة SelectArea مع معامل CellArea
                PivotAreaCollection selectedAreas = pivotTable.SelectArea(area);
                
                Console.WriteLine("SelectArea method executed successfully. Selected areas count: " + selectedAreas.Count);
                
                // احفظ المصنف لإظهار التأثير
                workbook.Save("PivotTableSelectAreaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SelectArea method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotAreaCollection](../../pivotareacollection/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


