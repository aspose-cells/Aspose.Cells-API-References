##Worksheet.CustomProperties
Worksheet property. Gets an object representing the identifier information associated with a worksheet
## Worksheet.CustomProperties property
Gets an object representing the identifier information associated with a worksheet.
```csharp
public CustomPropertyCollection CustomProperties { get; }
```
### Remarks
Worksheet.CustomProperties provide a preferred mechanism for storing arbitrary data. It supports legacy third-party document components, as well as those situations that have a stringent need for binary parts.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyCustomPropertiesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add custom properties to the worksheet
worksheet.CustomProperties.Add("Property1", "Value1");
worksheet.CustomProperties.Add("Property2", "12345");
worksheet.CustomProperties.Add("Property3", DateTime.Now.ToString());
// Display count of custom properties
Console.WriteLine("Custom Properties Count: " + worksheet.CustomProperties.Count);
// Access and display property values
foreach (var prop in worksheet.CustomProperties)
{
Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
}
// Save the workbook
workbook.Save("WorksheetCustomPropertiesDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
