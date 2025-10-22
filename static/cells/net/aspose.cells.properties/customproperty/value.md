##CustomProperty.Value
CustomProperty property. Returns or sets the value of the custom property
## CustomProperty.Value property
Returns or sets the value of the custom property.
```csharp
public string Value { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomPropertyPropertyValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a custom property with a long string value
worksheet.CustomProperties.Add("VeryLongString", "This is a very long string value for testing custom properties");
// Get and display the value of the custom property
string propertyValue = worksheet.CustomProperties["VeryLongString"].Value;
Console.WriteLine("Custom Property Value: " + propertyValue);
// Save the workbook
workbook.Save("output.xlsx");
// Reload the workbook to verify the property persists
Workbook loadedWorkbook = new Workbook("output.xlsx");
Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
// Verify the value is the same after loading
string loadedValue = loadedWorksheet.CustomProperties["VeryLongString"].Value;
Console.WriteLine("Reloaded Custom Property Value: " + loadedValue);
}
}
}
```
### See Also
* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
