##WorksheetCollection.XmlMaps
WorksheetCollection property. Gets and sets the XML maps in the workbook
## WorksheetCollection.XmlMaps property
Gets and sets the XML maps in the workbook.
```csharp
public XmlMapCollection XmlMaps { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyXmlMapsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a sample XML map
string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
// Add XML map to the workbook
int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
// Access the XML map
XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
// Export XML data (demonstrates XmlMaps property usage)
workbook.ExportXml(map.Name, "output.xml");
Console.WriteLine("XML exported successfully using XmlMaps property.");
}
}
}
```
### See Also
* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
