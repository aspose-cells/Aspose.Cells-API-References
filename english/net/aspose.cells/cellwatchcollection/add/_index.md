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
// Called: int watchIndex = sheet.CellWatches.Add(&amp;quot;B2&amp;quot;);
public static void Method_String_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Get the first Worksheet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add Cell Watch Item into the watch window
            int watchIndex = sheet.CellWatches.Add(&quot;B2&quot;);
            
            // Access the CellWatchCollection
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Access the added CellWatch item
            CellWatch cellWatch = cellWatches[watchIndex];
            
            // Display the properties of the CellWatch item
            Console.WriteLine(&quot;Cell Watch Details:&quot;);
            Console.WriteLine($&quot;Row: {cellWatch.Row}&quot;);
            Console.WriteLine($&quot;Column: {cellWatch.Column}&quot;);
            Console.WriteLine($&quot;Cell Name: {cellWatch.CellName}&quot;);
            
            // Modify the properties of the CellWatch item
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = &quot;A2&quot;;
            
            // Display the modified properties of the CellWatch item
            Console.WriteLine(&quot;Modified Cell Watch Details:&quot;);
            Console.WriteLine($&quot;Row: {cellWatch.Row}&quot;);
            Console.WriteLine($&quot;Column: {cellWatch.Column}&quot;);
            Console.WriteLine($&quot;Cell Name: {cellWatch.CellName}&quot;);
            
            // Save the workbook
            workbook.Save(&quot;CellWatchCollectionExample.xlsx&quot;);
            workbook.Save(&quot;CellWatchCollectionExample.pdf&quot;);
        }
```

### See Also

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


