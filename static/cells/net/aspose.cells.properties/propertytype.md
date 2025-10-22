##Enum PropertyType
Aspose.Cells.Properties.PropertyType enum. Specifies data type of a document property
## PropertyType enumeration
Specifies data type of a document property.
```csharp
public enum PropertyType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Boolean | `0` | The property is a boolean value. |
| DateTime | `1` | The property is a date time value. |
| Double | `2` | The property is a floating number. |
| Number | `3` | The property is an integer number. |
| String | `4` | The property is a string value. |
| Blob | `5` | The property is a byte array. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class PropertyTypeDemo
{
public static void PropertyTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set some built-in properties
builtInProperties.Author = "John Doe";
builtInProperties.Title = "Sample Workbook";
builtInProperties.Subject = "Demonstration of PropertyType";
builtInProperties.Company = "Aspose";
// Access the custom document properties
CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;
// Add custom properties of different types
customProperties.Add("IsReviewed", true); // Boolean
customProperties.Add("ReviewDate", DateTime.Now); // DateTime
customProperties.Add("Rating", 4.5); // Double
customProperties.Add("Pages", 100); // Number
customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String
// Retrieve and display custom properties
foreach (DocumentProperty property in customProperties)
{
Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
}
// Save the workbook
workbook.Save("PropertyTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)
