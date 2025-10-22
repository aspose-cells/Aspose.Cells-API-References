##CustomPropertyCollection.Item
CustomPropertyCollection property. Gets the custom property by the specific index
## CustomPropertyCollection indexer (1 of 2)
Gets the custom property by the specific index.
```csharp
public CustomProperty this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
The custom property
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class CustomPropertyCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
CustomPropertyCollection customProperties = sheet.CustomProperties;
customProperties.Add("Author", "John Doe");
customProperties.Add("Version", "1.0");
customProperties.Add("DateCreated", DateTime.Now.ToString("yyyy-MM-dd"));
for (int i = 0; i < customProperties.Count; i++)
{
CustomProperty property = customProperties[i];
Console.WriteLine($"Property {i}: {property.Name} = {property.Value}");
}
workbook.Save("CustomPropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
## CustomPropertyCollection indexer (2 of 2)
Gets the custom property by the property name.
```csharp
public CustomProperty this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The property name. |
### Return Value
The custom property
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomPropertyCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add custom properties
worksheet.CustomProperties.Add("COR_Report", "Quarterly Report");
worksheet.CustomProperties.Add("COR_ResultSet", "Sales Data");
// Access and display custom properties using Item property
Console.WriteLine("COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
Console.WriteLine("COR_ResultSet: " + worksheet.CustomProperties["COR_ResultSet"].Value);
// Modify a custom property using Item property
worksheet.CustomProperties["COR_Report"].Value = "Annual Report";
Console.WriteLine("Updated COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
}
}
}
```
### See Also
* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
