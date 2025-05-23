---
title: ListObject.DataSourceType
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the data source type of the table
type: docs
url: /net/aspose.cells.tables/listobject/datasourcetype/
---
## ListObject.DataSourceType property

Gets the data source type of the table.

```csharp
public TableDataSourceType DataSourceType { get; }
```

### Examples

```csharp
// Called: TableDataSourceType dataSourceType = listObject.DataSourceType;
public static void ListObject_Property_DataSourceType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Add a ListObject (table) to the worksheet
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Set the display name of the table
            listObject.DisplayName = "SampleTable";

            // Set the data source type of the table
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // Output the data source type
            Console.WriteLine("Data Source Type: " + dataSourceType);

            // Save the workbook
            workbook.Save("TableDataSourceTypeExample.xlsx");
        }
```

### See Also

* enum [TableDataSourceType](../../tabledatasourcetype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


