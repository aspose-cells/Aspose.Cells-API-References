##ExternalConnection.Credentials
ExternalConnection property. Specifies the authentication method to be used when establishing or reestablishing the connection
## ExternalConnection.Credentials property
Specifies the authentication method to be used when establishing (or re-establishing) the connection.
```csharp
[Obsolete("Use ExternalConnection.CredentialsMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CredentialsMethodType Credentials { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use ExternalConnection.CredentialsMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyCredentialsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current Credentials value
Console.WriteLine("Initial Credentials value: " + connection.Credentials);
// Set a new Credentials value (since it's read-write)
connection.Credentials = CredentialsMethodType.Integrated;
Console.WriteLine("Updated Credentials value: " + connection.Credentials);
// Cycle through possible values
foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
{
connection.Credentials = method;
Console.WriteLine($"Credentials set to: {method}");
}
// Save the workbook with the modified connection settings
workbook.Save("CredentialsDemo.xlsx");
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
* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
