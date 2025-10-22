##Workbook.ExportXml
Workbook method. Export XML data linked by the specified XML map
## ExportXml(string, string) {#exportxml_1}
Export XML data linked by the specified XML map.
```csharp
public void ExportXml(string mapName, string path)
```
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| path | String | the export path |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodExportXmlWithStringStringDemo
{
public static void Run()
{
// Create a workbook and load the Excel file
Workbook wb = new Workbook("Book1.xlsx");
// Get the first XmlMap from the workbook
if (wb.Worksheets.XmlMaps.Count > 0)
{
XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
// Export XML data using the XmlMap's name and output file path
wb.ExportXml(xmlMap.Name, "output.xml");
Console.WriteLine("XML exported successfully to output.xml");
}
else
{
Console.WriteLine("No XmlMap found in the workbook");
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ExportXml(string, Stream) {#exportxml}
Export XML data.
```csharp
public void ExportXml(string mapName, Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| stream | Stream | the export stream |
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
