##Class XmlMap
Aspose.Cells.XmlMap class. Represents Xml map information
## XmlMap class
Represents Xml map information.
```csharp
public class XmlMap
```
## Properties
| Name | Description |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | Gets an [`XmlDataBinding`](../xmldatabinding/) of this map. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | Returns or sets the name of the object. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | Gets root element name. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassXmlMapDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data to the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Item2");
worksheet.Cells["B3"].PutValue(200);
// Create an XML map from a sample XML string
string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
// Add the XML map to the workbook
int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
// Export data to XML using the map
workbook.ExportXml(xmlMap.Name, "output.xml");
Console.WriteLine("XML exported successfully using XmlMap.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
