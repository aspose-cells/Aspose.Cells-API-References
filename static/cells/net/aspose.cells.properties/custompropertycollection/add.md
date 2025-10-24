##CustomPropertyCollection.Add
CustomPropertyCollection method. Adds custom property information
## CustomPropertyCollection.Add method
Adds custom property information.
```csharp
public int Add(string name, string value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the custom property. |
| value | String | The value of the custom property. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class CustomPropertyCollectionMethodAddWithStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
CustomPropertyCollection customProperties = worksheet.CustomProperties;
customProperties.Add("Author", "John Doe");
customProperties.Add("Version", "1.0");
foreach (CustomProperty property in customProperties)
{
Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
}
workbook.Save("CustomPropertiesExample.xlsx");
}
}
}
```
### See Also
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
