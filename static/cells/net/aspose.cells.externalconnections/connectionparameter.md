##Class ConnectionParameter
Aspose.Cells.ExternalConnections.ConnectionParameter class. Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries
## ConnectionParameter class
Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.
```csharp
public class ConnectionParameter
```
## Properties
| Name | Description |
| --- | --- |
| [CellReference](../../aspose.cells.externalconnections/connectionparameter/cellreference/) { get; set; } | Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [Name](../../aspose.cells.externalconnections/connectionparameter/name/) { get; set; } | The name of the parameter. |
| [Prompt](../../aspose.cells.externalconnections/connectionparameter/prompt/) { get; set; } | Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt. |
| [RefreshOnChange](../../aspose.cells.externalconnections/connectionparameter/refreshonchange/) { get; set; } | Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
| [SqlType](../../aspose.cells.externalconnections/connectionparameter/sqltype/) { get; set; } | SQL data type of the parameter. Only valid for ODBC sources. |
| [Type](../../aspose.cells.externalconnections/connectionparameter/type/) { get; set; } | Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used. In this case, it is expected that only one of {boolean, double, integer, or string} will be specified. |
| [Value](../../aspose.cells.externalconnections/connectionparameter/value/) { get; set; } | Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionsClassConnectionParameterDemo
{
public static void Run()
{
// Create a new workbook for demonstration
Workbook workbook = new Workbook();
try
{
// Create a connection parameter using reflection since constructor isn't public
ConnectionParameter parameter = (ConnectionParameter)Activator.CreateInstance(typeof(ConnectionParameter), nonPublic: true);
// Set basic properties
parameter.Name = "CustomerID";
parameter.Type = ConnectionParameterType.Value;
parameter.Value = "CUST1001";
parameter.RefreshOnChange = true;
parameter.Prompt = "Enter Customer ID:";
// Display parameter information
Console.WriteLine($"Created parameter: {parameter.Name}");
Console.WriteLine($"Type: {parameter.Type}");
Console.WriteLine($"Value: {parameter.Value}");
Console.WriteLine($"Refresh on change: {parameter.RefreshOnChange}");
Console.WriteLine($"Prompt: {parameter.Prompt}");
// Save the workbook
workbook.Save("ConnectionParameterDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error working with ConnectionParameter: {ex.Message}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)
