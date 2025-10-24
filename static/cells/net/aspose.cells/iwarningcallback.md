##Interface IWarningCallback
Aspose.Cells.IWarningCallback interface. Callback interface of warning
## IWarningCallback interface
Callback interface of warning.
```csharp
public interface IWarningCallback
```
## Methods
| Name | Description |
| --- | --- |
| [Warning](../../aspose.cells/iwarningcallback/warning/)(WarningInfo) | Our callback only needs to implement the "Warning" method. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class IWarningCallbackDemo : IWarningCallback
{
// Implementing the Warning method from the IWarningCallback interface
public void Warning(WarningInfo warningInfo)
{
// Display the warning message
Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
}
public static void IWarningCallbackExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the warning callback
workbook.Settings.WarningCallback = new IWarningCallbackDemo();
// Load a workbook with potential warnings
try
{
workbook = new Workbook("example.xlsx");
}
catch (Exception ex)
{
Console.WriteLine("Exception: " + ex.Message);
}
// Save the workbook
workbook.Save("IWarningCallbackExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
