##OleObject.SetEmbeddedObject
OleObject method. Sets embedded object data
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}
Sets embedded object data.
```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName,
bool displayAsIcon, string label)
```
| Parameter | Type | Description |
| --- | --- | --- |
| linkToFile | Boolean | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| objectData | Byte[] | The embedded object data. |
| sourceFileName | String | The file name. |
| displayAsIcon | Boolean | Indicates whether diplaying object as an icon. If true, the orginal image data will be covered by icon. |
| label | String | The icon label. Only works when displayAsIcon as true. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OleObject to the worksheet
int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
OleObject oleObject = worksheet.OleObjects[oleObjectIndex];
try
{
// Prepare parameters for SetEmbeddedObject
bool linkToFile = false;
byte[] objectData = File.ReadAllBytes("sample.xlsx");
string sourceFileName = "sample.xlsx";
bool displayAsIcon = false;
string label = "Excel Document";
// Call SetEmbeddedObject with the specified parameters
oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label);
Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String)");
// Display some properties to show the effect
Console.WriteLine($"OleObject label: {oleObject.Label}");
Console.WriteLine($"Display as icon: {oleObject.DisplayAsIcon}");
Console.WriteLine($"Is linked to file: {oleObject.IsLink}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
}
// Save the workbook
workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}
Sets embedded object data.
```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName,
bool displayAsIcon, string label, bool updateIcon)
```
| Parameter | Type | Description |
| --- | --- | --- |
| linkToFile | Boolean | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| objectData | Byte[] | The embedded object data. |
| sourceFileName | String | The file name. |
| displayAsIcon | Boolean | Indicates whether diplaying object as an icon. If true, the orginal image data will be covered by icon. |
| label | String | The icon label. Only works when displayAsIcon as true. |
| updateIcon | Boolean | Indicates whether automatically updating icon. |
### Remarks
As Aspose can update embedd all file icons, so it's better that you can add correct icon with *updateIcon* as false.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OleObject to the worksheet
int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
OleObject oleObject = worksheet.OleObjects[oleObjectIndex];
try
{
// Prepare parameters for SetEmbeddedObject
bool linkToFile = false;
byte[] objectData = File.ReadAllBytes("sample.docx");
string sourceFileName = "sample.docx";
bool displayAsIcon = true;
string label = "Word Document";
bool updateIcon = true;
// Call SetEmbeddedObject with the specified parameters
oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon);
Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String, Boolean)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
}
// Save the workbook
workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
