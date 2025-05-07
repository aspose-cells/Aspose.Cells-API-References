---
title: FindOptions.SeachOrderByRows
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Indicates whether search order by rows or columns
type: docs
url: /net/aspose.cells/findoptions/seachorderbyrows/
---
## FindOptions.SeachOrderByRows property

Indicates whether search order by rows or columns.

```csharp
[Obsolete("Use FindOptions.SearchOrderByRows property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SeachOrderByRows { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use FindOptions.SearchOrderByRows property. This property will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: findOptions.SeachOrderByRows = true;
public static void Property_SeachOrderByRows()
        {
            // Instantiate the workbook object
            Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");

            // Get Cells collection 
            Cells cells = workbook.Worksheets[0].Cells;

            // Instantiate FindOptions Object
            FindOptions findOptions = new FindOptions();

            // Create a Cells Area
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;

            // Set cells area for find options
            findOptions.SetRange(ca);

            // Set searching properties
            findOptions.SearchBackward = false;
            findOptions.SeachOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Set LookAtType to Contains
            findOptions.LookAtType = LookAtType.Contains;

            // Find the cell with a specific value
            Cell cell = cells.Find("searchValue", null, findOptions);

            if (cell != null)
            {
                Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


