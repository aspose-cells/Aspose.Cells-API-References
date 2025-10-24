##DocumentProperty.ToDateTime
DocumentProperty method. Returns the property value as DateTime in local timezone
## DocumentProperty.ToDateTime method
Returns the property value as DateTime in local timezone.
```csharp
public DateTime ToDateTime()
```
### Remarks
Throws an exception if the property type is not PropertyType.Date.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class DocumentPropertyMethodToDateTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get custom document properties collection
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
// Add a datetime property
DateTime currentTime = DateTime.Now;
customProperties.Add("LastModified", currentTime);
// Get the property and convert to DateTime
DocumentProperty lastModifiedProperty = customProperties["LastModified"];
DateTime retrievedTime = lastModifiedProperty.ToDateTime();
// Output the result
Console.WriteLine($"Stored DateTime: {currentTime}");
Console.WriteLine($"Retrieved DateTime: {retrievedTime}");
// Save the workbook
workbook.Save("DocumentPropertyDateTimeExample.xlsx");
}
}
}
```
### See Also
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
