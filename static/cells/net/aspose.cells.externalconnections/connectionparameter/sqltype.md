##ConnectionParameter.SqlType
ConnectionParameter property. SQL data type of the parameter. Only valid for ODBC sources
## ConnectionParameter.SqlType property
SQL data type of the parameter. Only valid for ODBC sources.
```csharp
public SqlDataType SqlType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ConnectionParameterPropertySqlTypeDemo
{
public static void Run()
{
try
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a connection parameter (simulated since constructor parameters are unknown)
ConnectionParameter parameter = null;
// In a real scenario, you would create the parameter properly
// parameter = new ConnectionParameter(/* required parameters */);
// For demonstration, we'll show how SqlType would be used if we had a parameter
if (parameter != null)
{
// Get and display the current SqlType value
Console.WriteLine("Current SqlType: " + parameter.SqlType);
// Set a new SqlType value (since property is read-write)
parameter.SqlType = SqlDataType.SqlInteger;
Console.WriteLine("Updated SqlType: " + parameter.SqlType);
}
else
{
// Fallback demonstration when we can't create the parameter
workbook.Worksheets[0].Cells["A1"].Value = "SqlType property demo (see code comments)";
Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
}
// Save the workbook
workbook.Save("ConnectionParameterSqlTypeDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SqlDataType](../../sqldatatype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
