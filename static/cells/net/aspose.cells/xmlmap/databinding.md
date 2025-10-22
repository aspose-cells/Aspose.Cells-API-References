##XmlMap.DataBinding
XmlMap property. Gets an XmlDataBinding of this map
## XmlMap.DataBinding property
Gets an [`XmlDataBinding`](../../xmldatabinding/) of this map.
```csharp
public XmlDataBinding DataBinding { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlMapPropertyDataBindingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample XML maps
string url1 = "https://example.com/data1.xml";
string url2 = "https://example.com/data2.xml";
// Add first XML map
int mapIndex1 = workbook.Worksheets.XmlMaps.Add(url1);
XmlMap map1 = workbook.Worksheets.XmlMaps[mapIndex1];
// Add second XML map
int mapIndex2 = workbook.Worksheets.XmlMaps.Add(url2);
XmlMap map2 = workbook.Worksheets.XmlMaps[mapIndex2];
// Demonstrate DataBinding property usage
Console.WriteLine("First XML Map:");
Console.WriteLine("Name: " + map1.Name);
Console.WriteLine("Root Element: " + map1.RootElementName);
Console.WriteLine("Data Binding URL: " + map1.DataBinding.Url);
Console.WriteLine("\nSecond XML Map:");
Console.WriteLine("Name: " + map2.Name);
Console.WriteLine("Root Element: " + map2.RootElementName);
Console.WriteLine("Data Binding URL: " + map2.DataBinding.Url);
// Save the workbook
workbook.Save("XmlMapDataBindingDemo.xlsx");
}
}
}
```
### See Also
* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
