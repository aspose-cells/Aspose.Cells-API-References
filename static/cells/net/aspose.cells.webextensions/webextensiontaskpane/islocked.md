##WebExtensionTaskPane.IsLocked
WebExtensionTaskPane property. Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user
## WebExtensionTaskPane.IsLocked property
Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user.
```csharp
public bool IsLocked { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionTaskPanePropertyIsLockedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
try
{
// Create task pane through workbook's web extension collection
WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
int paneIndex = taskPanes.Add();
WebExtensionTaskPane taskPane = taskPanes[paneIndex];
Console.WriteLine("Initial IsLocked value: " + taskPane.IsLocked);
taskPane.IsLocked = true;
Console.WriteLine("Updated IsLocked value: " + taskPane.IsLocked);
workbook.Save("WebExtensionTaskPaneDemo.xlsx");
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
* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
