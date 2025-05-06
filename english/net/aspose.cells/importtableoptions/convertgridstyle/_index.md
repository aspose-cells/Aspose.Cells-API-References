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
public static void Property_ConvertGridStyle()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a DataTable to import
            DataTable dataTable = new DataTable(&quot;SampleData&quot;);
            dataTable.Columns.Add(&quot;ID&quot;, typeof(int));
            dataTable.Columns.Add(&quot;Name&quot;, typeof(string));
            dataTable.Columns.Add(&quot;Date&quot;, typeof(DateTime));
            dataTable.Rows.Add(1, &quot;John Doe&quot;, DateTime.Now);
            dataTable.Rows.Add(2, &quot;Jane Smith&quot;, DateTime.Now.AddDays(1));

            // Create an instance of ImportTableOptions
            ImportTableOptions importOptions = new ImportTableOptions
            {
                ConvertGridStyle = true,
                ConvertNumericData = true,
                InsertRows = true,
                ShiftFirstRowDown = false,
                IsFieldNameShown = true,
                ExportCaptionAsFieldName = false,
                DateFormat = &quot;yyyy-MM-dd&quot;,
                TotalRows = -1, // Import all rows
                TotalColumns = -1, // Import all columns
                IsHtmlString = false,
                CheckMergedCells = false
            };

            // Import the DataTable into the worksheet
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Save the workbook
            workbook.Save(&quot;ImportTableOptionsExample.xlsx&quot;);
            workbook.Save(&quot;ImportTableOptionsExample.pdf&quot;);
            return;
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


