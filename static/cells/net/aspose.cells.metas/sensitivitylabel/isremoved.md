##SensitivityLabel.IsRemoved
SensitivityLabel property. Indicates whether the sensitivity label was removed
## SensitivityLabel.IsRemoved property
Indicates whether the sensitivity label was removed.
```csharp
public bool IsRemoved { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
using System;
public class SensitivityLabelPropertyIsRemovedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a sensitivity label instance through reflection
// since direct instantiation isn't available
Type labelType = typeof(SensitivityLabel);
SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
// Set required properties
label.Id = "SENSITIVE_DATA";
label.IsEnabled = true;
label.IsRemoved = false;
// Display initial IsRemoved value
Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
// Demonstrate setting the IsRemoved property (since it's read-write)
label.IsRemoved = true;
Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
// Toggle the value back to show it can be changed
label.IsRemoved = false;
Console.WriteLine("Final IsRemoved value: " + label.IsRemoved);
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
