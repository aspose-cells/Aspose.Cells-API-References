##Class SensitivityLabel
Aspose.Cells.Metas.SensitivityLabel class. Represents the sensitivity label
## SensitivityLabel class
Represents the sensitivity label.
```csharp
public class SensitivityLabel
```
## Properties
| Name | Description |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | Gets and sets the assignment method for the sensitivity label. |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | Gets and sets the types of content marking that ought to be applied to a file. |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | Gets and sets the id of sensitivity label. |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | Indicates whether the sensitivity label is enabled |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | Indicates whether the sensitivity label was removed. |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | Represents the Azure Active Directory (Azure AD) site identifier corresponding to the sensitivity label policy which describes the sensitivity label. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
using System;
public class MetasClassSensitivityLabelDemo
{
public static void Run()
{
// Create a new workbook for demonstration
Workbook workbook = new Workbook();
try
{
// Create an instance of the SensitivityLabel class using reflection
SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
// Set basic properties
label.Id = "CONFIDENTIAL_001";
label.IsEnabled = true;
label.AssignmentType = SensitivityLabelAssignmentType.Standard;
label.ContentMarkType = SensitivityLabelMarkType.None;
// Display property values
Console.WriteLine($"Sensitivity Label Created:");
Console.WriteLine($"ID: {label.Id}");
Console.WriteLine($"Enabled: {label.IsEnabled}");
Console.WriteLine($"Assignment Type: {label.AssignmentType}");
Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
// Save the workbook
workbook.Save("SensitivityLabelDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error working with SensitivityLabel: {ex.Message}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)
