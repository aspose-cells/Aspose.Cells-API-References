---
title: ImportTableOptions.ConvertGridStyle
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether apply the style of the grid view to cells
type: docs
url: /net/aspose.cells/importtableoptions/convertgridstyle/
---
## ImportTableOptions.ConvertGridStyle property

Indicates whether apply the style of the grid view to cells.

```csharp
public bool ConvertGridStyle { get; set; }
```

### Examples

```csharp
// Called: ConvertGridStyle = true,
public static void ImportTableOptions_Property_ConvertGridStyle()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a DataTable to import
            DataTable dataTable = new DataTable("SampleData");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Date", typeof(DateTime));
            dataTable.Rows.Add(1, "John Doe", DateTime.Now);
            dataTable.Rows.Add(2, "Jane Smith", DateTime.Now.AddDays(1));

            // Create an instance of ImportTableOptions
            ImportTableOptions importOptions = new ImportTableOptions
            {
                ConvertGridStyle = true,
                ConvertNumericData = true,
                InsertRows = true,
                ShiftFirstRowDown = false,
                IsFieldNameShown = true,
                ExportCaptionAsFieldName = false,
                DateFormat = "yyyy-MM-dd",
                TotalRows = -1, // Import all rows
                TotalColumns = -1, // Import all columns
                IsHtmlString = false,
                CheckMergedCells = false
            };

            // Import the DataTable into the worksheet
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Save the workbook
            workbook.Save("ImportTableOptionsExample.xlsx");
            workbook.Save("ImportTableOptionsExample.pdf");
            return;
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


