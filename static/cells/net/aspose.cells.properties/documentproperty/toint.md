##DocumentProperty.ToInt
DocumentProperty method. Returns the property value as integer
## DocumentProperty.ToInt method
Returns the property value as integer.
```csharp
public int ToInt()
```
### Remarks
Throws an exception if the property type is not PropertyType.Number.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class DocumentPropertyMethodToIntDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the custom document properties collection
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
// Add a numeric custom property
customProperties.Add("Revision", 5);
// Get the property and convert to int using ToInt()
DocumentProperty revisionProperty = customProperties["Revision"];
int revisionValue = revisionProperty.ToInt();
// Output the result
Console.WriteLine($"Revision (as int): {revisionValue}");
// Save the workbook
workbook.Save("DocumentPropertyToIntExample.xlsx");
}
}
}
```
### See Also
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
