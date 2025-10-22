##Class WorkbookDesigner
Aspose.Cells.WorkbookDesigner class. Encapsulates the object that represents a designer spreadsheet
## WorkbookDesigner class
Encapsulates the object that represents a designer spreadsheet.
```csharp
public class WorkbookDesigner
```
## Constructors
| Name | Description |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | Initializes a new instance of the `WorkbookDesigner` class. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | Initializes a new instance of the `WorkbookDesigner` class. |
## Properties
| Name | Description |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | Indicates whether formulas should be calculated. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | Gets and sets callback interface of processing smartmarker. |
| [ContainsVariables](../../aspose.cells/workbookdesigner/containsvariables/) { get; set; } | (**Obsolete.**) Indicates whether the first worksheet contains custom variables. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | (**Obsolete.**) Indicates whether processing the smart marker line by line. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | Indicates whether repeating formulas with subtotal row. |
| [SortDataSource](../../aspose.cells/workbookdesigner/sortdatasource/) { get; set; } | Indicates whether sorting data source. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | If TRUE, Null will be inserted if the value is ""; |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | Indicates if references in other worksheets will be updated. |
| [VariablesWorksheetName](../../aspose.cells/workbookdesigner/variablesworksheetname/) { get; set; } | Gets and sets the name of the worksheet which contains variables smart marker. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | Gets and sets the [`Workbook`](./workbook/) object. |
## Methods
| Name | Description |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | Clears all data sources. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | Returns a collection of smart markers in a spreadsheet. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | Processes the smart markers and populates the data source values. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | Processes the smart markers and populates the data source values. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | Processes the smart markers and populates the data source values. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | (**Obsolete.**) Processes the smart markers and populates the data source values. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | Sets data source of a DataSet object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | Sets data source of a DataTable object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | Sets data source of a DataView object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | Sets data source of a OleDbConnection object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | Sets data source of a SqlConnection object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | Sets data source of a DataView object and binds it to a data source name. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | Sets data source of a [`ICellsDataTable`](../icellsdatatable/) object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | Sets data binding to a variable. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | Sets data source of a IDataReader object. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) | Set json string value as data source of smart markers. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Data;
public class WorkbookDesignerDemo
{
public static void WorkbookDesignerExample()
{
// Create WorkbookDesigner object
WorkbookDesigner wd = new WorkbookDesigner();
// Open the template file (which contains smart markers)
wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");
// Initialize your data from data source
DataSet ds = new DataSet();
// Add data to the dataset (this is just an example, replace with actual data source)
DataTable dt = new DataTable("Table1");
dt.Columns.Add("Column1");
dt.Columns.Add("Column2");
dt.Rows.Add("Value1", "Value2");
dt.Rows.Add("Value11", "Value22");
ds.Tables.Add(dt);
// Set the dataset as the data source
wd.SetDataSource(ds);
// Process the smart markers to fill the data into the worksheets
wd.Process(true);
// Save the excel file
wd.Workbook.Save("WorkbookDesignerExample.xlsx");
// Demonstrating other properties
wd.RepeatFormulasWithSubtotal = true;
wd.UpdateEmptyStringAsNull = true;
wd.UpdateReference = true;
wd.CalculateFormula = true;
wd.LineByLine = true;
// Clear data source
wd.ClearDataSource();
// Set data source using different methods
wd.SetDataSource("dataSourceName", dt);
wd.SetDataSource(dt);
wd.SetDataSource(ds);
wd.SetDataSource("dataSourceName", new DataView(dt));
wd.SetDataSource(new DataView(dt));
wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
wd.SetDataSource("variable", new object());
// Process the smart markers again
wd.Process();
wd.Process(true);
wd.Process(0, true);
// Save the excel file again
wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
