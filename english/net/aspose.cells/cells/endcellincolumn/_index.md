---
title: Cells.EndCellInColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the last cell in this column
type: docs
url: /net/aspose.cells/cells/endcellincolumn/
---
## EndCellInColumn(int) {#endcellincolumn}

Gets the last cell in this column.

```csharp
public Cell EndCellInColumn(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |

### Return Value

Cell object.

### Examples

```csharp
// Called: Cell lastDCell = wb_demo.Worksheets[0].Cells.EndCellInColumn((short)0);
public void Cells_Method_EndCellInColumn()
{
    string filePath = Constants.PivotTableSourcePath + @"JAVA41817_";

    Workbook wb_demo = new Workbook(filePath + "Book2.xlsx");
    PivotTable pt_demo = wb_demo.Worksheets[0].PivotTables[0];
    pt_demo.ColumnFields[0].ShowAllItems = true;
    pt_demo.DataFields[0].ShowAllItems = true;

    PivotField src_t_field = pt_demo.PageFields[0];
    src_t_field.IsMultipleItemSelectionAllowed = true;
    //pt_demo.getColumnFields().get(0).setShowAllItems(true); 

    pt_demo.RefreshData();

    PivotItemCollection collection_src_t = src_t_field.PivotItems;

    for (int i = 0; i < collection_src_t.Count; i++)
    {
        PivotItem item = collection_src_t[i];
        Console.WriteLine(item.Name);
        if ((item.Name != null) && item.Name.Equals("CCC"))
        {
            Console.WriteLine(item.Name + " src selected");
            item.IsHidden = false;
        }
        else
        {
            item.IsHidden = true;
        }
    }
    pt_demo.RefreshData();
    pt_demo.CalculateData();

    for (int i = 0; i < pt_demo.BaseFields.Count; i++)
    {
        pt_demo.BaseFields[i].ShowAllItems = true;
        Console.WriteLine(pt_demo.BaseFields[i].Name);
    }
    /* 
    pt_demo.getColumnFields().get(0).setShowAllItems(true); 
    System.out.println(pt_demo.getColumnFields().get(0).getName()); 
    pt_demo.getDataFields().get(0).setShowAllItems(true); 
    System.out.println(pt_demo.getDataFields().get(0).getName()); 
    pt_demo.getRowFields().get(0).setShowAllItems(true); 
    System.out.println(pt_demo.getRowFields().get(0).getName()); 
    pt_demo.getDataFields().get(0).setShowAllItems(true); 
    System.out.println(pt_demo.getDataFields().get(0).getName()); 
    */

    pt_demo.RowFields[0].ShowAllItems = true;
    Console.WriteLine(pt_demo.RowFields[0].Name);

    pt_demo.RefreshData();
    pt_demo.CalculateData();

    Cell lastDCell = wb_demo.Worksheets[0].Cells.EndCellInColumn((short)0);

    for (int row = 1; row <= lastDCell.Row; row++)
    {
        //System.out.println(row+" "+lastFCell.getRow()); 
        Cell cell0 = wb_demo.Worksheets[0].Cells[row, 0];
        Cell cell1 = wb_demo.Worksheets[0].Cells[row, 1];
        Cell cell2 = wb_demo.Worksheets[0].Cells[row, 2];
        Cell cell3 = wb_demo.Worksheets[0].Cells[row, 3];
        Cell cell4 = wb_demo.Worksheets[0].Cells[row, 4];

        Console.WriteLine("Demo " + cell0.Value + " "
                + cell1.Value + " "
                + cell2.Value + " "
                + cell3.Value + " "
                + cell4.Value + " "
                );

    }
    Assert.AreEqual(wb_demo.Worksheets[0].Cells[4, 0].StringValue, "xxx");
    Assert.AreEqual(wb_demo.Worksheets[0].Cells[5, 0].StringValue, "yyy");
    Assert.AreEqual(wb_demo.Worksheets[0].Cells[6, 0].StringValue, "zzz");
    wb_demo.Save(Constants.PivotTableDestPath + @"example.xlsx");
}
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EndCellInColumn(int, int, int, int) {#endcellincolumn_1}

Gets the last cell with maximum column index in this range.

```csharp
public Cell EndCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
| startColumn | Int32 | Start column index. |
| endColumn | Int32 | End column index. |

### Return Value

Cell object.

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate data in column B (index 1)
            worksheet.Cells[0, 1].PutValue("Data 1");
            worksheet.Cells[2, 1].PutValue("Data 2");
            worksheet.Cells[3, 1].PutValue("Data 3");

            try
            {
                // Call EndCellInColumn with parameters: startRow=0, endRow=5, startColumn=1, endColumn=1
                Cell result = worksheet.Cells.EndCellInColumn(0, 5, 1, 1);

                if (result != null)
                {
                    Console.WriteLine($"Last cell in column B between rows 0-5 is at row {result.Row}, column {result.Column}");
                    // Mark the found cell
                    result.PutValue("Last Cell");
                    Style style = result.GetStyle();
                    style.Font.IsBold = true;
                    result.SetStyle(style);
                }
                else
                {
                    Console.WriteLine("No cells found in specified range");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInColumn method: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


