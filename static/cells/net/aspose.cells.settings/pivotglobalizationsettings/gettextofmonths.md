##PivotGlobalizationSettings.GetTextOfMonths
PivotGlobalizationSettings method. Gets the local text of Months
## PivotGlobalizationSettings.GetTextOfMonths method
Gets the local text of "Months".
```csharp
public virtual string GetTextOfMonths()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfMonthsDemo
{
public static void Run()
{
// Create custom globalization settings
var customSettings = new CustomPivotGlobalizationSettings();
// Demonstrate GetTextOfMonths
Console.WriteLine("Custom Months Text: " + customSettings.GetTextOfMonths());
}
}
public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
{
public override string GetTextOfMonths()
{
// Return custom localized text for "Months"
return "Custom Months Label";
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)
