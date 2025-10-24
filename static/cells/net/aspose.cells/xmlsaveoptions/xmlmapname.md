##XmlSaveOptions.XmlMapName
XmlSaveOptions property. Indicates whether exporting xml map in the file
## XmlSaveOptions.XmlMapName property
Indicates whether exporting xml map in the file.
```csharp
public string XmlMapName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlSaveOptionsPropertyXmlMapNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill some data in the worksheet
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(999.99);
// Create XML map and add it to the workbook
int mapIndex = workbook.Worksheets.XmlMaps.Add("<Schema><Element><Product/><Price/></Element></Schema>");
XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
xmlMap.Name = "ProductDataMap";
// Create XmlSaveOptions and set XmlMapName
XmlSaveOptions saveOptions = new XmlSaveOptions();
saveOptions.XmlMapName = "ProductDataMap";
// Save the workbook with XML mapping
workbook.Save("XmlWithMapping.xml", saveOptions);
}
}
}
```
### See Also
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
