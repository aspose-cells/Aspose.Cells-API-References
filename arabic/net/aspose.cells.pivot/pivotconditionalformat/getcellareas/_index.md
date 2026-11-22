---
title: "PivotConditionalFormat.GetCellAreas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotConditionalFormat. تحصل على جميع مناطق الخلايا التي يُطبق عليها هذا التنسيق الشرطي"
type: docs
url: /ar/net/aspose.cells.pivot/pivotconditionalformat/getcellareas/
---
## PivotConditionalFormat.GetCellAreas method

يحصل على جميع مناطق الخلايا التي يُطبق عليها هذا التنسيق الشرطي.

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

    public class PivotConditionalFormatMethodGetCellAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء جدول محوري مطلوب لـ PivotConditionalFormat
                worksheet.Cells["A1"].Value = "Header";
                worksheet.Cells["A2"].Value = "Data";
                int pivotIndex = worksheet.PivotTables.Add("A1:A2", "B3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // إنشاء تنسيق شرطي عبر مجموعة الجدول المحوري
                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat conditionalFormat = pivotTable.ConditionalFormats[formatIndex];
                
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 2;
                area.EndColumn = 2;
                conditionalFormat.AddCellArea(area);

                CellArea[] resultAreas = conditionalFormat.GetCellAreas();
                
                Console.WriteLine($"Retrieved {resultAreas.Length} cell area(s):");
                foreach (CellArea ca in resultAreas)
                {
                    Console.WriteLine($"Rows {ca.StartRow}-{ca.EndRow}, Cols {ca.StartColumn}-{ca.EndColumn}");
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
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


