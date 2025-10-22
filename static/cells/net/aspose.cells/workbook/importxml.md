##Workbook.ImportXml
Workbook method. Imports/Updates an XML data file into the workbook
## ImportXml(string, string, int, int) {#importxml_1}
Imports/Updates an XML data file into the workbook.
```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```
| Parameter | Type | Description |
| --- | --- | --- |
| url | String | the url/path of the xml file. |
| sheetName | String | the destination sheet name. |
| row | Int32 | the destination row |
| col | Int32 | the destination column |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
{
public static void Run()
{
// Create a workbook object
Workbook wb = new Workbook();
// Import XML data into the first worksheet starting at cell A1
wb.ImportXml("data.xml", "Sheet1", 0, 0);
// Save the workbook
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportXml(Stream, string, int, int) {#importxml}
Imports/Updates an XML data file into the workbook.
```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | the xml file stream. |
| sheetName | String | the destination sheet name. |
| row | Int32 | the destination row. |
| col | Int32 | the destination column. |
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
