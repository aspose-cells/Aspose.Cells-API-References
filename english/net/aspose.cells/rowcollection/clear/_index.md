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
public static void RowCollection_Method_Clear()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("Aspose.Cells");
            // Get the Rows collection
            RowCollection rows = worksheet.Cells.Rows;

            // Get the number of rows in the collection
            int rowCount = rows.Count;
            Console.WriteLine("Number of rows: " + rowCount);

            // Get the first row
            Row firstRow = rows[0];
            Console.WriteLine("First row index: " + firstRow.Index);

            // Iterate through the rows using GetEnumerator
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
            }

            // Get a row by index
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine("Specific row index: " + specificRow.Index);

            // Clear all rows and cells
            rows.Clear();
            Console.WriteLine("Rows cleared.");

            // Save the workbook
            workbook.Save("RowCollectionExample.xlsx");
        }
```

### See Also

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


