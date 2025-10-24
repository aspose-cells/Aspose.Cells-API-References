##PivotGlobalizationSettings.GetTextOfYears
PivotGlobalizationSettings method. Gets the local text of Years
## PivotGlobalizationSettings.GetTextOfYears method
Gets the local text of "Years".
```csharp
public virtual string GetTextOfYears()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfYearsDemo
{
public static void Run()
{
// Create custom globalization settings
var customSettings = new CustomPivotGlobalizationSettings();
// Demonstrate GetTextOfYears method
Console.WriteLine("Custom Text of Years: " + customSettings.GetTextOfYears());
}
}
public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
{
public override string GetTextOfYears()
{
// Return custom text for "Years" label
return "Custom Years Label";
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)
