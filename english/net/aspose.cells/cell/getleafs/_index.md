---
title: Cell.GetLeafs
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Get all cells which reference to this cell directly and need to be updated when this cell is modified
type: docs
url: /net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

Get all cells which reference to this cell directly and need to be updated when this cell is modified.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### Return Value

Enumerator to enumerate all dependents(Cell)

### Remarks

NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data and formulas to create dependencies
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Get the cell that has dependents
                Cell cell = worksheet.Cells["B1"];

                // Call GetLeafs to get all cells that reference this cell directly
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // Save the workbook
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

Get all cells which will be updated when this cell is modified.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| Parameter | Type | Description |
| --- | --- | --- |
| recursive | Boolean | Whether returns those leafs that do not reference to this cell directly but reference to other leafs of this cell |

### Return Value

Enumerator to enumerate all dependents(Cell)

### Remarks

NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data with formulas to create dependencies
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Get the cell that has dependents
                Cell cell = worksheet.Cells["A1"];

                // Call GetLeafs with recursive parameter set to true
                IEnumerator leafs = cell.GetLeafs(true);

                // Display the results
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // Save the workbook
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


