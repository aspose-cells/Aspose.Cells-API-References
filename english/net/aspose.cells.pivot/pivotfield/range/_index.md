---
title: PivotField.Range
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Gets the group range of the pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/range/
---
## PivotField.Range property

Gets the group range of the pivot field

```csharp
[Obsolete("Use PivotField.GroupSettings property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SxRng Range { get; }
```

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GroupSettings property. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: SxRng range = columnField.Range;
public static void PivotField_Property_Range()
        {
            // Create a new workbook
            Workbook workbook = new Workbook("SxRngExample_original.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];


            PivotTableCollection pivotTables = worksheet.PivotTables;
            PivotTable pivotTable = pivotTables[0];


            // Access the first column field
            PivotField columnField = pivotTable.ColumnFields[0];

            // Access the range of the pivot field
            SxRng range = columnField.Range;

            // Display properties of the SxRng object
            Console.WriteLine("IsAutoStart: " + range.IsAutoStart);
            Console.WriteLine("IsAutoEnd: " + range.IsAutoEnd);
            Console.WriteLine("Start: " + range.Start);
            Console.WriteLine("End: " + range.End);
            Console.WriteLine("By: " + range.By);

            // Save the workbook
            workbook.Save("SxRngExample.xlsx");
        }
```

### See Also

* class [SxRng](../../sxrng/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


