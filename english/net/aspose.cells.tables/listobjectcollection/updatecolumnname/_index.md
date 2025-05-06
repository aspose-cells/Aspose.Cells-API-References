---
title: ListObjectCollection.UpdateColumnName
second_title: Aspose.Cells for .NET API Reference
description: ListObjectCollection method. Update all column name of the tables
type: docs
url: /net/aspose.cells.tables/listobjectcollection/updatecolumnname/
---
## ListObjectCollection.UpdateColumnName method

Update all column name of the tables.

```csharp
public void UpdateColumnName()
```

### Examples

```csharp
// Called: listObjects.UpdateColumnName();
public static void Method_UpdateColumnName()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the ListObjectCollection of the worksheet
            ListObjectCollection listObjects = worksheet.ListObjects;

            // Add a ListObject (table) to the worksheet
            int listObjectIndex = listObjects.Add(0, 0, 10, 4, true);
            ListObject listObject = listObjects[listObjectIndex];

            // Set the name of the ListObject
            listObject.DisplayName = &quot;SampleTable&quot;;

            // Populate the table with some data
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Header1&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Header2&quot;);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Header3&quot;);
            worksheet.Cells[&quot;D1&quot;].PutValue(&quot;Header4&quot;);

            for (int i = 1; i &lt;= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(&quot;Row&quot; + i + &quot;Col1&quot;);
                worksheet.Cells[i, 1].PutValue(&quot;Row&quot; + i + &quot;Col2&quot;);
                worksheet.Cells[i, 2].PutValue(&quot;Row&quot; + i + &quot;Col3&quot;);
                worksheet.Cells[i, 3].PutValue(&quot;Row&quot; + i + &quot;Col4&quot;);
            }

            // Update all column names of the tables
            listObjects.UpdateColumnName();

            // Save the workbook
            workbook.Save(&quot;ListObjectCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


