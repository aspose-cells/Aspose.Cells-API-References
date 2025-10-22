##CustomXmlPartCollection.Add
CustomXmlPartCollection method. Adds an item to the collection
## CustomXmlPartCollection.Add method
Adds an item to the collection.
```csharp
public int Add(byte[] data, byte[] shemaData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| data | Byte[] | The XML content of this Custom XML Data Storage Part. |
| shemaData | Byte[] | The set of XML schemas that are associated with this custom XML part. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
using System.Text;
public class CustomXmlPartCollectionMethodAddWithByteByteDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the CustomXmlPartCollection directly from workbook
CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
// Prepare XML data and schema as byte arrays
string xmlData = "<root><item>Test Data</item></root>";
string schemaData = "<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'><xs:element name='root'><xs:complexType><xs:sequence><xs:element name='item' type='xs:string'/></xs:sequence></xs:complexType></xs:element></xs:schema>";
byte[] xmlBytes = Encoding.UTF8.GetBytes(xmlData);
byte[] schemaBytes = Encoding.UTF8.GetBytes(schemaData);
try
{
// Call the Add method with byte array parameters
int index = customXmlParts.Add(xmlBytes, schemaBytes);
Console.WriteLine($"Custom XML part added successfully at index: {index}");
// Save the workbook to demonstrate the effect
workbook.Save("CustomXmlPartAddDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error adding custom XML part: {ex.Message}");
}
}
}
}
```
### See Also
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
