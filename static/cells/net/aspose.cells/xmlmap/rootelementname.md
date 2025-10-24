##XmlMap.RootElementName
XmlMap property. Gets root element name
## XmlMap.RootElementName property
Gets root element name.
```csharp
public string RootElementName { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlMapPropertyRootElementNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue(100);
// Create an XML map
string xml = "<root><item><Name>Item1</Name><Value>100</Value></item></root>";
int mapIndex = workbook.Worksheets.XmlMaps.Add(xml);
// Get and display the root element name
string rootElementName = workbook.Worksheets.XmlMaps[mapIndex].RootElementName;
Console.WriteLine("Root Element Name: " + rootElementName);
}
}
}
```
### See Also
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
