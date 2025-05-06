---
title: RowCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: RowCollection method. Clear all rows and cells
type: docs
url: /net/aspose.cells/rowcollection/clear/
---
## RowCollection.Clear method

Clear all rows and cells.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: rows.Clear();
public static void Method_Clear()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;World&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Aspose.Cells&quot;);
            // Get the Rows collection
            RowCollection rows = worksheet.Cells.Rows;

            // Get the number of rows in the collection
            int rowCount = rows.Count;
            Console.WriteLine(&quot;Number of rows: &quot; + rowCount);

            // Get the first row
            Row firstRow = rows[0];
            Console.WriteLine(&quot;First row index: &quot; + firstRow.Index);

            // Iterate through the rows using GetEnumerator
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine(&quot;Row index: &quot; + row.Index + &quot;, Height: &quot; + row.Height);
            }

            // Get a row by index
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine(&quot;Specific row index: &quot; + specificRow.Index);

            // Clear all rows and cells
            rows.Clear();
            Console.WriteLine(&quot;Rows cleared.&quot;);

            // Save the workbook
            workbook.Save(&quot;RowCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


