---
title: CellWatchCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: CellWatchCollection method. Adds CellWatch with row and column
type: docs
url: /net/aspose.cells/cellwatchcollection/add/
---
## Add(int, int) {#add}

Adds [`CellWatch`](../../cellwatch/) with row and column.

```csharp
public int Add(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Return Value

Returns the position of this item in the collection.

### See Also

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Adds [`CellWatch`](../../cellwatch/) with the name the of cell.

```csharp
public int Add(string cellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |

### Examples

```csharp
// Called: int watchIndex = sheet.CellWatches.Add("B2");
public static void Method_String_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            // Get the first Worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Add Cell Watch Item into the watch window
            int watchIndex = sheet.CellWatches.Add("B2");

            // Retrieve the CellWatch object
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Setting properties
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // Save the workbook
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
```

### See Also

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


