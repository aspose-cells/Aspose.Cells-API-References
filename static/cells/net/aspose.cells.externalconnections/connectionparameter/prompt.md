##ConnectionParameter.Prompt
ConnectionParameter property. Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType  prompt
## ConnectionParameter.Prompt property
Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt.
```csharp
public string Prompt { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ConnectionParameterPropertyPromptDemo
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
// For demonstration, we'll show how Prompt would be used if we had a parameter
if (parameter != null)
{
// Get and display the current Prompt value
Console.WriteLine("Current Prompt: " + parameter.Prompt);
// Set a new Prompt value (since property is read-write)
parameter.Prompt = "Enter customer ID:";
Console.WriteLine("Updated Prompt: " + parameter.Prompt);
}
else
{
// Fallback demonstration when we can't create the parameter
workbook.Worksheets[0].Cells["A1"].Value = "Prompt property demo (see code comments)";
Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
}
// Save the workbook
workbook.Save("ConnectionParameterPromptDemo.xlsx");
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
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
