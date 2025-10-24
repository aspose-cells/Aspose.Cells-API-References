##Enum ConnectionParameterType
Aspose.Cells.ExternalConnections.ConnectionParameterType enum. Specifies the parameter type of external connection
## ConnectionParameterType enumeration
Specifies the parameter type of external connection
```csharp
public enum ConnectionParameterType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Cell | `0` | Get the parameter value from a cell on each refresh. |
| Prompt | `1` | Prompt the user on each refresh for a parameter value. |
| Value | `2` | Use a constant value on each refresh for the parameter value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionsClassConnectionParameterTypeDemo
{
public static void Run()
{
try
{
// Demonstrate creating and using ConnectionParameterType enum values
ConnectionParameterType cellParam = ConnectionParameterType.Cell;
ConnectionParameterType promptParam = ConnectionParameterType.Prompt;
ConnectionParameterType valueParam = ConnectionParameterType.Value;
// Display the enum values
Console.WriteLine("Connection Parameter Types:");
Console.WriteLine($"Cell: {cellParam}");
Console.WriteLine($"Prompt: {promptParam}");
Console.WriteLine($"Value: {valueParam}");
// Demonstrate usage in a switch statement
ConnectionParameterType testParam = ConnectionParameterType.Prompt;
switch (testParam)
{
case ConnectionParameterType.Cell:
Console.WriteLine("Parameter will get value from a cell");
break;
case ConnectionParameterType.Prompt:
Console.WriteLine("Parameter will prompt user for value");
break;
case ConnectionParameterType.Value:
Console.WriteLine("Parameter will use constant value");
break;
}
}
catch (Exception ex)
{
Console.WriteLine($"Error demonstrating ConnectionParameterType: {ex.Message}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)
