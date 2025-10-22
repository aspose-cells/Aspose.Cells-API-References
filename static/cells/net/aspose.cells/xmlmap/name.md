##XmlMap.Name
XmlMap property. Returns or sets the name of the object
## XmlMap.Name property
Returns or sets the name of the object.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlMapPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["B2"].PutValue("John Doe");
// Add an XML map
string xmlSchema = "<xs:schema xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">" +
"<xs:element name=\"Employee\">" +
"<xs:complexType><xs:sequence>" +
"<xs:element name=\"ID\" type=\"xs:int\"/>" +
"<xs:element name=\"Name\" type=\"xs:string\"/>" +
"</xs:sequence></xs:complexType></xs:element></xs:schema>";
int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
map.Name = "Employee";
// Demonstrate using the Name property
Console.WriteLine("XML Map Name: " + map.Name);
// Export to XML using the map's name
string savePath = "output.xml";
workbook.ExportXml(map.Name, savePath);
Console.WriteLine("XML exported successfully to: " + savePath);
}
}
}
```
### See Also
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
