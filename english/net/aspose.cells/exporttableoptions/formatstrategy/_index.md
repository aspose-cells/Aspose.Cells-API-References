---
title: ExportTableOptions.FormatStrategy
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Gets and sets the format strategy when exporting the value as string value
type: docs
url: /net/aspose.cells/exporttableoptions/formatstrategy/
---
## ExportTableOptions.FormatStrategy property

Gets and sets the format strategy when exporting the value as string value.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Examples

```csharp
// Called: FormatStrategy = CellValueFormatStrategy.DisplayStyle,
public static void ExportTableOptions_Property_FormatStrategy()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells[0, 0].PutValue("Name");
            worksheet.Cells[0, 1].PutValue("Age");
            worksheet.Cells[1, 0].PutValue("John");
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue("Jane");
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
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Save the workbook
            workbook.Save("ExportTableOptionsExample.xlsx");
            workbook.Save("ExportTableOptionsExample.pdf");
        }
```

### See Also

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


