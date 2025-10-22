##DataModelConnection.CommandType
DataModelConnection property. Returns OLEDBCommandType type
## DataModelConnection.CommandType property
Returns [`OLEDBCommandType`](../../oledbcommandtype/) type.
```csharp
public override OLEDBCommandType CommandType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.QueryTables;
using System;
using System.Collections.Generic;
using System.Runtime.Serialization;
public class DataModelConnectionPropertyCommandTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Create DataModelConnection instance using uninitialized object
DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
((IList<ExternalConnection>)workbook.DataConnections).Add(connection);
Console.WriteLine("Current CommandType value: " + connection.CommandType);
connection.CommandType = OLEDBCommandType.SqlStatement;
connection.Command = "SELECT * FROM Customers";
connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
// Create PowerQueryFormula using uninitialized object and set properties
PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
query.Name = "SampleQuery";
typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
((IList<PowerQueryFormula>)queries).Add(query);
workbook.Save("PropertyCommandTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
