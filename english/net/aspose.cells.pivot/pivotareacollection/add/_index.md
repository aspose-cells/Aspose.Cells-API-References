---
title: PivotAreaCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: PivotAreaCollection method. Adds pivot area
type: docs
url: /net/aspose.cells.pivot/pivotareacollection/add/
---
## Add(PivotArea) {#add}

Adds pivot area.

```csharp
[Obsolete("Use PivotAreaCollection.AddPivotArea(PivotArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(PivotArea pivotArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | PivotArea | The pivot area. |

### Remarks

NOTE: This member is now obsolete. Instead, please use AddPivotArea() method. This method will be removed 6 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotAreaCollectionMethodAddWithPivotAreaDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("PivotTable");
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Add pivot table
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // Add fields to pivot areas
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Create conditional format
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;

            // Create pivot area and add to collection
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            pcf.PivotAreas.Add(pivotArea);

            // Add format condition
            FormatCondition fc = pcf.FormatConditions[pcf.FormatConditions.AddCondition(FormatConditionType.CellValue)];
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Formula1 = "15";
            fc.Style.BackgroundColor = Color.Yellow;

            // Calculate data and save
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotAreaCollectionMethodAddWithPivotAreaDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Adds an area based on pivot table view.

```csharp
public void Add(CellArea cellArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | The area based on pivot table view. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data for pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Add a pivot table
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Define a cell area to add to pivot areas
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 0;
            cellArea.StartColumn = 0;
            cellArea.EndRow = 2;
            cellArea.EndColumn = 1;

            // Get pivot area collection by selecting the area
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea);

            try
            {
                // Call the Add method with CellArea parameter
                pivotAreas.Add(cellArea);

                Console.WriteLine("Pivot area added successfully for cell area: " +
                    $"({cellArea.StartRow},{cellArea.StartColumn}) to ({cellArea.EndRow},{cellArea.EndColumn})");

                // Display the added pivot areas
                foreach (PivotArea area in pivotAreas)
                {
                    CellArea[] areas = area.GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Pivot area covers: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Save the result
            workbook.Save("PivotAreaCollectionMethodAddWithCellAreaDemo.xlsx");
        }
    }
}
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


