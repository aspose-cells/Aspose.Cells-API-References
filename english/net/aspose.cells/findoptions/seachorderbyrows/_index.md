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
            Workbook workbook = new Workbook(&quot;FindOptionsExample_original.xlsx&quot;);

            // Get Cells collection 
            Cells cells = workbook.Worksheets[0].Cells;

            // Instantiate FindOptions Object
            FindOptions findOptions = new FindOptions();

            // Create a Cells Area
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 5;
            ca.EndColumn = 5;

            // Set cells area for find options
            findOptions.SetRange(ca);

            // Set searching properties
            findOptions.SearchBackward = false;
            findOptions.SeachOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Find the cell with 0 value
            Cell cell = cells.Find(0, null, findOptions);

            if (cell != null)
            {
                Console.WriteLine(&quot;Cell found at: &quot; + cell.Name);
            }
            else
            {
                Console.WriteLine(&quot;Cell not found.&quot;);
            }
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


