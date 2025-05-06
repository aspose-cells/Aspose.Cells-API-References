---
title: ExportTableOptions.AllowDBNull
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. This value indicates whether DBNulls are allowed in this table
type: docs
url: /net/aspose.cells/exporttableoptions/allowdbnull/
---
## ExportTableOptions.AllowDBNull property

This value indicates whether DBNulls are allowed in this table.

```csharp
public bool AllowDBNull { get; set; }
```

### Examples

```csharp
// Called: AllowDBNull = true,
public static void Property_AllowDBNull()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells[0, 0].PutValue(&quot;Name&quot;);
            worksheet.Cells[0, 1].PutValue(&quot;Age&quot;);
            worksheet.Cells[1, 0].PutValue(&quot;John&quot;);
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue(&quot;Jane&quot;);
            worksheet.Cells[2, 1].PutValue(25);

            // Create an instance of ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                SkipErrorValue = true,
                PlotVisibleCells = true,
                PlotVisibleRows = true,
                PlotVisibleColumns = true,
                ExportAsString = false,
                ExportAsHtmlString = false,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                CheckMixedValueType = true,
                AllowDBNull = true,
                IsVertical = true,
                RenameStrategy = RenameStrategy.Digit
            };

            // Export the data from the worksheet to a DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Display the exported data
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + &quot;\t&quot;);
                }
                Console.WriteLine();
            }

            // Save the workbook
            workbook.Save(&quot;ExportTableOptionsExample.xlsx&quot;);
            workbook.Save(&quot;ExportTableOptionsExample.pdf&quot;);
        }
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


