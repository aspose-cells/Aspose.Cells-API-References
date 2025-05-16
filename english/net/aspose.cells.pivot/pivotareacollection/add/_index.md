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
public int Add(PivotArea pivotArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | PivotArea | The pivot area. |

### Examples

```csharp
// Called: pcf.PivotAreas.Add(pivotArea);
public void PivotAreaCollection_Method_Add()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    PivotTableCollection pivotTables;
    PivotTable pivotTable;
    PivotField pivotField;
    PivotItemCollection pivotItems;
    PivotItem pivotItem;
    PivotFieldCollection pivotDataFields;

    int pivotTableIndex;

    Worksheet detailWorksheet = workbook.Worksheets["Detail"];


    Worksheet worksheet = workbook.Worksheets.Add("RENEWALS WITH LR >= 40%");
    worksheet.TabColor = Color.Red;

    pivotTables = worksheet.PivotTables;

    pivotTableIndex = pivotTables.Add($"'Detail'!A1:{CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, detailWorksheet.Cells.MaxDataColumn)}", "A1", "PivotTable1");

    pivotTable = pivotTables[pivotTableIndex];

    pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight16;

    pivotTable.ShowValuesRow = false;

    //RowFields
    pivotTable.AddFieldToArea(PivotFieldType.Row, "MonthDay");

    //Uncheck "(blank)" item
    pivotField = pivotTable.RowFields["MonthDay"];
    pivotField.IsAutoSort = true;
    pivotField.IsAscendSort = true;

    pivotItems = pivotField.PivotItems;

    for (int i = 0; i < pivotItems.Count; i++)
    {
        pivotItem = pivotItems[i];
        if (pivotItem.Name != null && pivotItem.Name.Equals("(blank)"))
        {
            pivotItem.IsHidden = true;
        }
    }

    pivotTable.AddFieldToArea(PivotFieldType.Row, "CommonName");

    pivotTable.AddFieldToArea(PivotFieldType.Row, "PolicyNumber");
    pivotField = pivotTable.RowFields["PolicyNumber"];
    //Hide Subtotal
    pivotField.IsAutoSubtotals = false;

    pivotTable.AddFieldToArea(PivotFieldType.Row, "CoveragePart");
    pivotField = pivotTable.RowFields["CoveragePart"];
    //Hide Subtotal
    pivotField.IsAutoSubtotals = false;

    pivotTable.AddFieldToArea(PivotFieldType.Row, "ExpDate");
    pivotField = pivotTable.RowFields["ExpDate"];
    //Hide Subtotal
    pivotField.IsAutoSubtotals = false;

    pivotTable.AddFieldToArea(PivotFieldType.Row, "ClaimCount");

    //DataFields
    pivotTable.AddFieldToArea(PivotFieldType.Data, "Written");
    pivotTable.AddFieldToArea(PivotFieldType.Data, "Earned");
    pivotTable.AddFieldToArea(PivotFieldType.Data, "Incurred");


    //Calculated fields
    pivotTable.AddCalculatedField("Inc to Earned LR", "('Incurred'/'Earned')");

    pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);

    //Update Captions and NumberFormats
    pivotDataFields = pivotTable.DataFields;

    pivotDataFields["Written"].DisplayName = "Written";
    pivotDataFields["Written"].NumberFormat = @"_($* #,##0.00_);_($* (#,##0.00);_($* "" - ""??_);_(@_)";

    pivotDataFields["Earned"].DisplayName = "Earned";
    pivotDataFields["Earned"].NumberFormat = @"_($* #,##0.00_);_($* (#,##0.00);_($* "" - ""??_);_(@_)";

    pivotDataFields["Incurred"].DisplayName = "Incurred";
    pivotDataFields["Incurred"].NumberFormat = @"_($* #,##0.00_);_($* (#,##0.00);_($* "" - ""??_);_(@_)";

    pivotDataFields["Inc to Earned LR"].DisplayName = "Inc to Earned LR %";
    pivotDataFields["Inc to Earned LR"].NumberFormat = "0.00%";


    //Conditional format Loss Ratio >= 40%
    PivotConditionalFormatCollection pcfCollection = pivotTable.ConditionalFormats;
    pcfCollection.Clear();
    worksheet.ConditionalFormattings.Clear();

    PivotConditionalFormat pcf = pcfCollection[pcfCollection.Add()];
    pcf.ScopeType = PivotConditionFormatScopeType.Field;

    PivotArea pivotArea = new PivotArea(pivotTable);
    pivotArea.SelectField(PivotFieldType.Data, "Inc to Earned LR");
    pivotArea.SelectField(PivotFieldType.Row, "CommonName");
    pcf.PivotAreas.Add(pivotArea);
    Assert.IsTrue(pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic));

    //pcf.AddFieldArea(PivotFieldType.Data, "Inc to Earned LR");
    //pcf.AddFieldArea(PivotFieldType.Row, "CommonName");

    FormatConditionCollection fcc = pcf.FormatConditions;
    int idx = fcc.AddCondition(FormatConditionType.CellValue);
    FormatCondition fc = fcc[idx];
    fc.Formula1 = "0.4";
    fc.Operator = OperatorType.GreaterOrEqual;
    fc.Style.BackgroundArgbColor = Color.FromArgb(255, 199, 206).ToArgb();
    fc.Style.Font.ArgbColor = Color.FromArgb(156, 0, 6).ToArgb();


    pivotTable.RefreshData();
    pivotTable.CalculateData();
    pivotTable.RefreshDataOnOpeningFile = true;

    //Autofit all columns and rows
    worksheet.AutoFitColumns();
    worksheet.AutoFitRows();
    workbook.Save(Constants.destPath + "example.xlsx");
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
namespace AsposeCellsExamples.PivotAreaCollectionMethodAddWithCellAreaDemo
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


