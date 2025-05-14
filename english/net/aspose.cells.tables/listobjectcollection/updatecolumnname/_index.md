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
public static void ListObjectCollection_Method_UpdateColumnName()
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
            listObject.DisplayName = "SampleTable";

            // Populate the table with some data
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["D1"].PutValue("Header4");

            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row" + i + "Col1");
                worksheet.Cells[i, 1].PutValue("Row" + i + "Col2");
                worksheet.Cells[i, 2].PutValue("Row" + i + "Col3");
                worksheet.Cells[i, 3].PutValue("Row" + i + "Col4");
            }

            // Update all column names of the tables
            listObjects.UpdateColumnName();

            // Save the workbook
            workbook.Save("ListObjectCollectionExample.xlsx");

            return;
        }
```

### See Also

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


