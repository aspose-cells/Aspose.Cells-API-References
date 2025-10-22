##PivotGlobalizationSettings.GetTextOfQuarters
PivotGlobalizationSettings method. Get the local text of Quarters
## PivotGlobalizationSettings.GetTextOfQuarters method
Get the local text of "Quarters".
```csharp
public virtual string GetTextOfQuarters()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfQuartersDemo
{
public static void Run()
{
// Create globalization settings instance
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
// Demonstrate GetTextOfQuarters method
Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
// Show other related time period labels for context
Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)
