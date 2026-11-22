---
title: "PivotArea.GetCellAreas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotArea. تحصل على مناطق الخلايا لهذه PivotArea"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/getcellareas/
---
## PivotArea.GetCellAreas method

يحصل على مناطق الخلايا في هذه المنطقة المحورية.

```csharp
public CellArea[] GetCellAreas()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaMethodGetCellAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات جدول محوري بسيطة
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";

            try
            {
                // إنشاء جدول محوري مع تكوين أساسي
                int pivotIndex = worksheet.PivotTables.Add("A1:A3", "D1", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // تهيئة PivotArea باستخدام مثيل جدول Pivot
                PivotArea pivotArea = new PivotArea(pivotTable);

                // تكوين إعدادات منطقة Pivot
                pivotArea.RuleType = PivotAreaType.Normal;
                pivotArea.AxisType = PivotFieldType.Data;
                pivotArea.IsRowGrandIncluded = true;

                // تنفيذ الطريقة المستهدفة
                CellArea[] cellAreas = pivotArea.GetCellAreas();

                Console.WriteLine($"GetCellAreas returned {cellAreas.Length} cell area(s)");
                foreach (CellArea area in cellAreas)
                {
                    Console.WriteLine($"CellArea: Columns {area.StartColumn}-{area.EndColumn}, Rows {area.StartRow}-{area.EndRow}");
                }

                workbook.Save("GetCellAreasDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetCellAreas: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


