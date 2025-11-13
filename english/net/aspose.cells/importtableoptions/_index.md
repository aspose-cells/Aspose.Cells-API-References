---
title: Class ImportTableOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ImportTableOptions class. Represents the options of importing data into cells
type: docs
url: /net/aspose.cells/importtableoptions/
---
## ImportTableOptions class

Represents the options of importing data into cells.

```csharp
public class ImportTableOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ImportTableOptions](importtableoptions/)() | Creates the default importing options. |

## Properties

| Name | Description |
| --- | --- |
| [CheckMergedCells](../../aspose.cells/importtableoptions/checkmergedcells/) { get; set; } | Indicates whether checking merged cells. |
| [ColumnIndexes](../../aspose.cells/importtableoptions/columnindexes/) { get; set; } | Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [ConvertGridStyle](../../aspose.cells/importtableoptions/convertgridstyle/) { get; set; } | Indicates whether apply the style of the grid view to cells. |
| [ConvertNumericData](../../aspose.cells/importtableoptions/convertnumericdata/) { get; set; } | Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [DateFormat](../../aspose.cells/importtableoptions/dateformat/) { get; set; } | Gets or sets date format string for cells with imported datetime values. |
| [DefaultValues](../../aspose.cells/importtableoptions/defaultvalues/) { get; set; } | Default value for the value in the table is null. |
| [ExportCaptionAsFieldName](../../aspose.cells/importtableoptions/exportcaptionasfieldname/) { get; set; } | Indicates whether exporting caption as field name |
| [InsertRows](../../aspose.cells/importtableoptions/insertrows/) { get; set; } | Indicates whether new rows should be added for importing data records. |
| [IsFieldNameShown](../../aspose.cells/importtableoptions/isfieldnameshown/) { get; set; } | Indicates whether field name should be imported. |
| [IsFormulas](../../aspose.cells/importtableoptions/isformulas/) { get; set; } | Indicates whether the data are formulas. |
| [IsHtmlString](../../aspose.cells/importtableoptions/ishtmlstring/) { get; set; } | Indicates whether the value contains html tags. |
| [NumberFormats](../../aspose.cells/importtableoptions/numberformats/) { get; set; } | Gets or sets the number formats |
| [ShiftFirstRowDown](../../aspose.cells/importtableoptions/shiftfirstrowdown/) { get; set; } | Indicates whether shifting the first row down when inserting rows. |
| [Styles](../../aspose.cells/importtableoptions/styles/) { get; set; } | Gets and sets the styles for each column of the table. |
| [TotalColumns](../../aspose.cells/importtableoptions/totalcolumns/) { get; set; } | Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [TotalRows](../../aspose.cells/importtableoptions/totalrows/) { get; set; } | Gets or sets total row count to import from data source. -1 means all rows of given data source. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsDemo
    {
        public static void ImportTableOptionsExample()
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
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


