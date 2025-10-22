##ExternalConnection.Type
ExternalConnection property. Gets or Sets the external connection DataSource type
## ExternalConnection.Type property
Gets or Sets the external connection DataSource type.
```csharp
[Obsolete("Use ExternalConnection.SourceType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ConnectionDataSourceType Type { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use ExternalConnection.SourceType property. This property will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current Type value (read operation)
Console.WriteLine("Initial Type value: " + connection.Type);
// Set a new Type value (since it's read-write)
connection.Type = ConnectionDataSourceType.OLEDBBasedSource;
Console.WriteLine("Updated Type value: " + connection.Type);
// Cycle through possible values to demonstrate setting capability
foreach (ConnectionDataSourceType type in Enum.GetValues(typeof(ConnectionDataSourceType)))
{
if ((int)type != 102) // Skip duplicate enum value
{
connection.Type = type;
Console.WriteLine($"Type set to: {type}");
}
}
// Save the workbook with the modified connection settings
workbook.Save("TypeDemo.xlsx");
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
* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
