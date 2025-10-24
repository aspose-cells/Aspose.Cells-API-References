##SensitivityLabel.ContentMarkType
SensitivityLabel property. Gets and sets the types of content marking that ought to be applied to a file
## SensitivityLabel.ContentMarkType property
Gets and sets the types of content marking that ought to be applied to a file.
```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
using System;
public class SensitivityLabelPropertyContentMarkTypeDemo
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
// Demonstrate ContentMarkType property (read-write)
Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
// Set different content mark types
label.ContentMarkType = SensitivityLabelMarkType.Header;
Console.WriteLine("After setting Header: " + label.ContentMarkType);
label.ContentMarkType = SensitivityLabelMarkType.Watermark;
Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
// Show combined flags usage
label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
// Save the workbook
workbook.Save("ContentMarkTypeDemo.xlsx");
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
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)
