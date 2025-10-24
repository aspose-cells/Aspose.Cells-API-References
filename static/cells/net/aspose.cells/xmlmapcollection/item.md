##XmlMapCollection.Item
XmlMapCollection property. Gets the xml map by the specific index
## XmlMapCollection indexer
Gets the xml map by the specific index.
```csharp
public XmlMap this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
The xml map
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlMapCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the XmlMapCollection from the workbook
XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;
// Add a new XmlMap to the collection
int xmlMapIndex = xmlMaps.Add("data.xsd");
// Access the XmlMap using Item property
XmlMap xmlMap = xmlMaps[xmlMapIndex];
// Display the XmlMap's name
Console.WriteLine("XmlMap Name: " + xmlMap.Name);
// Save the workbook
workbook.Save("XmlMapCollectionExample.xlsx");
}
}
}
```
### See Also
* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
