##PivotGlobalizationSettings.GetTextOfHours
PivotGlobalizationSettings method. Gets the local text of Hours
## PivotGlobalizationSettings.GetTextOfHours method
Gets the local text of "Hours".
```csharp
public virtual string GetTextOfHours()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfHoursDemo
{
public static void Run()
{
// Create an instance of PivotGlobalizationSettings
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
// Demonstrate the GetTextOfHours method
Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
// Additional demonstration of related time methods
Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)
