##SensitivityLabel.IsEnabled
SensitivityLabel property. Indicates whether the sensitivity label is enabled
## SensitivityLabel.IsEnabled property
Indicates whether the sensitivity label is enabled
```csharp
public bool IsEnabled { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
using System;
public class SensitivityLabelPropertyIsEnabledDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a sensitivity label instance
SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
// Set initial properties
label.Id = "CONFIDENTIAL_001";
// Demonstrate getting the initial IsEnabled value
Console.WriteLine("Initial IsEnabled value: " + label.IsEnabled);
// Set IsEnabled to true and display the change
label.IsEnabled = true;
Console.WriteLine("After enabling: " + label.IsEnabled);
// Toggle the value to demonstrate it's read-write
label.IsEnabled = false;
Console.WriteLine("After disabling: " + label.IsEnabled);
// Save the workbook
workbook.Save("IsEnabledDemo.xlsx");
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
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)
