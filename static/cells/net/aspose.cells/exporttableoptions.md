##Class ExportTableOptions
Aspose.Cells.ExportTableOptions class. Represents all export table options
## ExportTableOptions class
Represents all export table options.
```csharp
public class ExportTableOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [ExportTableOptions](exporttableoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [AllowDBNull](../../aspose.cells/exporttableoptions/allowdbnull/) { get; set; } | This value indicates whether DBNulls are allowed in this table. |
| [CheckMixedValueType](../../aspose.cells/exporttableoptions/checkmixedvaluetype/) { get; set; } | False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance. True, Aspose.Cells will check whether the value type in the column are mixed before set the DataColumn's type And the value type are mixed, the DataColumn's type will be string. |
| [DataTable](../../aspose.cells/exporttableoptions/datatable/) { get; set; } | Gets and sets the DataTable which columns' data type is assigned. |
| [ExportAsHtmlString](../../aspose.cells/exporttableoptions/exportashtmlstring/) { get; set; } | Exports the html string value of the cells to the DataTable. |
| [ExportAsString](../../aspose.cells/exporttableoptions/exportasstring/) { get; set; } | Exports the string value of the cells to the DataTable. |
| [ExportColumnName](../../aspose.cells/exporttableoptions/exportcolumnname/) { get; set; } | Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false. |
| [FormatStrategy](../../aspose.cells/exporttableoptions/formatstrategy/) { get; set; } | Gets and sets the format strategy when exporting the value as string value. |
| [Indexes](../../aspose.cells/exporttableoptions/indexes/) { get; set; } | The indexes of columns/rows which should be exported out. |
| [IsVertical](../../aspose.cells/exporttableoptions/isvertical/) { get; set; } | True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable. |
| [PlotVisibleCells](../../aspose.cells/exporttableoptions/plotvisiblecells/) { get; set; } | Only exports visible cells. |
| [PlotVisibleColumns](../../aspose.cells/exporttableoptions/plotvisiblecolumns/) { get; set; } | Only exports visible columns. |
| [PlotVisibleRows](../../aspose.cells/exporttableoptions/plotvisiblerows/) { get; set; } | Only exports visible rows. |
| [RenameStrategy](../../aspose.cells/exporttableoptions/renamestrategy/) { get; set; } | Strategy for duplicate names of columns. |
| [SkipErrorValue](../../aspose.cells/exporttableoptions/skiperrorvalue/) { get; set; } | Indicates whether skip invalid value for the column. For example,if the column type is decimal ,the value is greater than decimal.MaxValue and this property is true,we will not throw exception again. The default value is false. |
## Methods
| Name | Description |
| --- | --- |
| virtual [PreprocessExportedValue](../../aspose.cells/exporttableoptions/preprocessexportedvalue/)(int, int, CellValue) | Preprocess the value of current cell to be exported. |
### Remarks
If there are some special requirements about the exporting, such as ignoring error values, user may extend this class to overwrite corresponding apis to achive the goal.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Data;
public class ExportTableOptionsDemo
{
public static void ExportTableOptionsExample()
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
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
