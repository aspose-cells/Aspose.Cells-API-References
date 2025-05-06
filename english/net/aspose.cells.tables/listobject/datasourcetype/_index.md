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
public static void Property_DataSourceType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;ID&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(1);
            worksheet.Cells[&quot;A3&quot;].PutValue(2);
            worksheet.Cells[&quot;A4&quot;].PutValue(3);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Name&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(&quot;Alice&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(&quot;Bob&quot;);
            worksheet.Cells[&quot;B4&quot;].PutValue(&quot;Charlie&quot;);

            // Add a ListObject (table) to the worksheet
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Set the display name of the table
            listObject.DisplayName = &quot;SampleTable&quot;;

            // Set the data source type of the table
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // Output the data source type
            Console.WriteLine(&quot;Data Source Type: &quot; + dataSourceType);

            // Save the workbook
            workbook.Save(&quot;TableDataSourceTypeExample.xlsx&quot;);
        }
```

### See Also

* enum [TableDataSourceType](../../tabledatasourcetype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


