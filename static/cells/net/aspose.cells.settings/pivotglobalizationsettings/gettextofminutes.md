##PivotGlobalizationSettings.GetTextOfMinutes
PivotGlobalizationSettings method. Gets the local text of Minutes
## PivotGlobalizationSettings.GetTextOfMinutes method
Gets the local text of "Minutes".
```csharp
public virtual string GetTextOfMinutes()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfMinutesDemo
{
public static void Run()
{
// Create an instance of PivotGlobalizationSettings
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
// Demonstrate the GetTextOfMinutes method
Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
// Additional demonstration of related time methods for context
Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)
