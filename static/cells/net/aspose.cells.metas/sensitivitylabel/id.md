##SensitivityLabel.Id
SensitivityLabel property. Gets and sets the id of sensitivity label
## SensitivityLabel.Id property
Gets and sets the id of sensitivity label.
```csharp
public string Id { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
using System;
public class SensitivityLabelPropertyIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a sensitivity label instance
Type labelType = typeof(SensitivityLabel);
SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
// Demonstrate setting and getting the Id property
string testId = "CONFIDENTIAL_001";
label.Id = testId;
// Display the Id value
Console.WriteLine("Sensitivity Label Id: " + label.Id);
// Change the Id value to demonstrate it's read-write
label.Id = "INTERNAL_USE_ONLY";
Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
// Show the property affects other operations
label.IsEnabled = true;
Console.WriteLine($"Label {label.Id} is enabled: {label.IsEnabled}");
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
