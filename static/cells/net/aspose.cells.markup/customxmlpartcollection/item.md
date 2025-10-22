##CustomXmlPartCollection.Item
CustomXmlPartCollection property. Gets an item at the specified index
## CustomXmlPartCollection indexer
Gets an item at the specified index.
```csharp
public CustomXmlPart this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class CustomXmlPartCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the CustomXmlPartCollection directly from Workbook
CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
// Sample XML data
string xmlData = "<root><item>Test Data</item></root>";
byte[] xmlBytes = System.Text.Encoding.UTF8.GetBytes(xmlData);
// Add a custom XML part
int index = customXmlParts.Add(xmlBytes, null);
// Access the item using the Item property
CustomXmlPart part = customXmlParts[index];
// Display the ID of the custom XML part
Console.WriteLine("Custom XML Part ID: " + part.ID);
// Get the XML data back from the part
string retrievedXml = System.Text.Encoding.UTF8.GetString(part.Data);
Console.WriteLine("XML Content: " + retrievedXml);
// Save the workbook
workbook.Save("CustomXmlPartDemo.xlsx");
}
}
}
```
### See Also
* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
