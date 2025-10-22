##XmlMapCollection.Add
XmlMapCollection method. Add a XmlMap by the url/path of a xml/xsd file
## XmlMapCollection.Add method
Add a [`XmlMap`](../../xmlmap/) by the url/path of a xml/xsd file.
```csharp
public int Add(string url)
```
| Parameter | Type | Description |
| --- | --- | --- |
| url | String | url/path of a xml/xsd file. |
### Return Value
[`XmlMap`](../../xmlmap/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlMapCollectionMethodAddWithStringDemo
{
public static void Run()
{
Workbook wb = new Workbook();
XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;
// Add XML maps using schema and XML files
xmlMapCollection.Add("schema.xsd");
xmlMapCollection.Add("xml.xml");
wb.Save("twoXmlMaps.xlsx");
}
}
}
```
### See Also
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
