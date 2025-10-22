##Interface ISmartMarkerCallBack
Aspose.Cells.ISmartMarkerCallBack interface. Represents callback interface of processing smartmarker
## ISmartMarkerCallBack interface
Represents callback interface of processing smartmarker.
```csharp
public interface ISmartMarkerCallBack
```
## Methods
| Name | Description |
| --- | --- |
| [Process](../../aspose.cells/ismartmarkercallback/process/)(int, int, int, string, string) | Callback for processing a smart marker. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ISmartMarkerCallBackDemo : ISmartMarkerCallBack
{
// Implementing the Process method from ISmartMarkerCallBack interface
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
{
// Example implementation of the Process method
Console.WriteLine($"Processing sheetIndex: {sheetIndex}, rowIndex: {rowIndex}, colIndex: {colIndex}, tableName: {tableName}, columnName: {columnName}");
}
public static void ISmartMarkerCallBackExample()
{
// Create a new WorkbookDesigner instance
WorkbookDesigner designer = new WorkbookDesigner();
// Open a template file (which contains smart markers)
designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");
// Set the callback interface
designer.CallBack = new ISmartMarkerCallBackDemo();
// Initialize your data from data source
// For demonstration, we will use a simple DataTable
System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
dataTable.Columns.Add("Column1", typeof(string));
dataTable.Rows.Add("Value1");
dataTable.Rows.Add("Value2");
// Set the datatable as the data source
designer.SetDataSource(dataTable);
// Process the smart markers to fill the data into the worksheets
designer.Process(true);
// Save the excel file
designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
