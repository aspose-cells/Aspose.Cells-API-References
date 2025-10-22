##SensitivityLabel.AssignmentType
SensitivityLabel property. Gets and sets the assignment method for the sensitivity label
## SensitivityLabel.AssignmentType property
Gets and sets the assignment method for the sensitivity label.
```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
using System;
public class SensitivityLabelPropertyAssignmentTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a sensitivity label instance
SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
// Set basic properties
label.Id = "CONFIDENTIAL_001";
label.IsEnabled = true;
// Demonstrate getting the initial AssignmentType value
Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
// Set AssignmentType to Privileged and display the change
label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
Console.WriteLine("After setting Privileged: " + label.AssignmentType);
// Change back to Standard to demonstrate it's read-write
label.AssignmentType = SensitivityLabelAssignmentType.Standard;
Console.WriteLine("After setting Standard: " + label.AssignmentType);
// Save the workbook
workbook.Save("AssignmentTypeDemo.xlsx");
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
* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)
