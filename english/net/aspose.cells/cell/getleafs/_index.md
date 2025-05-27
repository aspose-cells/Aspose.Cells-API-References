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
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Set value in cell A1
                Cell cellA1 = worksheet.Cells["A1"];
                cellA1.PutValue(100);

                // Create dependent cell with formula referencing A1
                Cell cellB1 = worksheet.Cells["B1"];
                cellB1.Formula = "=A1*2";

                // Calculate workbook formulas to establish dependencies
                workbook.CalculateFormula();

                // Get leaf cells dependent on A1 using GetLeafs()
                IEnumerator dependentCells = cellA1.GetLeafs();
                Console.WriteLine("Cells immediately dependent on A1:");

                bool foundDependents = false;
                while (dependentCells.MoveNext())
                {
                    if (dependentCells.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"Dependent cell: {dependentCell.Name}");
                        foundDependents = true;
                    }
                }

                if (!foundDependents)
                {
                    Console.WriteLine("No direct dependent cells found");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLeafs method: {ex.Message}");
            }

            // Save the workbook to demonstrate persisted state
            workbook.Save("CellMethodGetLeafsDemo.xlsx");
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
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set up initial cell with value
            Cell sourceCell = worksheet.Cells["B2"];
            sourceCell.PutValue(100);

            // Create dependent cells with formulas
            worksheet.Cells["C3"].Formula = "=B2*1.1";
            worksheet.Cells["D4"].Formula = "=B2*0.9";
            worksheet.Cells["E5"].Formula = "=C3+D4";

            try
            {
                // Get all cells directly dependent on B2 with recursive=false
                IEnumerator dependents = sourceCell.GetLeafs(false);

                Console.WriteLine("Immediate dependents of B2:");
                while (dependents.MoveNext())
                {
                    if (dependents.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"Dependent cell: {dependentCell.Name}");
                        dependentCell.PutValue("Updated"); // Mark affected cells
                    }
                }

                // Calculate formulas to show dependency effect
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLeafs method: {ex.Message}");
            }

            workbook.Save("CellMethodGetLeafsWithBooleanDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


