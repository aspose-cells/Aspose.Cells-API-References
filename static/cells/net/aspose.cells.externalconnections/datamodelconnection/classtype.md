##DataModelConnection.ClassType
DataModelConnection property. Gets the type of this ExternalConnection object
## DataModelConnection.ClassType property
Gets the type of this [`ExternalConnection`](../../externalconnection/) object.
```csharp
public override ExternalConnectionClassType ClassType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.QueryTables;
using System;
using System.Runtime.Serialization;
public class DataModelConnectionPropertyClassTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create DataModelConnection instance using uninitialized object
DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
((IList<ExternalConnection>)workbook.DataConnections).Add(connection);
// Display the current ClassType value (read-only property)
Console.WriteLine("Current ClassType value: " + connection.ClassType);
// Set up connection properties
connection.Command = "SELECT * FROM Products";
connection.CommandType = OLEDBCommandType.SqlStatement;
connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
// Demonstrate how the ClassType affects connection handling
if (connection.ClassType == ExternalConnectionClassType.DataModel)
{
Console.WriteLine("This is a Data Model connection");
// Add PowerQueryFormula for data model connection
PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
query.Name = "ProductQuery";
typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
((IList<PowerQueryFormula>)queries).Add(query);
}
// Save the workbook
workbook.Save("DataModelConnectionClassTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
