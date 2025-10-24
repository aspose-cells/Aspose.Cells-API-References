##Cells.LinkToXmlMap
Cells method. Link to a xml map
## Cells.LinkToXmlMap method
Link to a xml map.
```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of xml map |
| row | Int32 | row of the destination cell |
| column | Int32 | column of the destination cell |
| path | String | path of xml element in xml map |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodLinkToXmlMapWithStringInt32Int32StringDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Add a sample XML map
int mapIndex = wb.Worksheets.XmlMaps.Add("<Transmittals><Issued_Document>Test</Issued_Document></Transmittals>");
XmlMap xmlMap = wb.Worksheets.XmlMaps[mapIndex];
xmlMap.Name = "Transmittals_Map";
// Get the first worksheet
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Link cell to XML map
cells.LinkToXmlMap("Transmittals_Map", 0, 0, "/Transmittals/Issued_Document");
// Save the workbook
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
