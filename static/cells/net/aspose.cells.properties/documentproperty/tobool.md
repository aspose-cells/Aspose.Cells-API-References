##DocumentProperty.ToBool
DocumentProperty method. Returns the property value as bool
## DocumentProperty.ToBool method
Returns the property value as bool.
```csharp
public bool ToBool()
```
### Remarks
Throws an exception if the property type is not PropertyType.Boolean.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class DocumentPropertyMethodToBoolDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
// Add a boolean custom document property
customProperties.Add("IsApproved", true);
// Get the property and convert to bool using ToBool()
DocumentProperty isApprovedProperty = customProperties["IsApproved"];
bool isApproved = isApprovedProperty.ToBool();
Console.WriteLine($"Is Approved: {isApproved}");
}
}
}
```
### See Also
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
