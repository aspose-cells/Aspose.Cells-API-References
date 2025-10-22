##OleObjectCollection.Add
OleObjectCollection method. Adds an OleObject to the collection
## Add(int, int, int, int, byte[]) {#add}
Adds an OleObject to the collection.
```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int height, int width, byte[] imageData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| height | Int32 | Height of oleObject, in unit of pixel. |
| width | Int32 | Width of oleObject, in unit of pixel. |
| imageData | Byte[] | Image of ole object as byte array. |
### Return Value
[`OleObject`](../../oleobject/) object index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare OLE object data (sample Excel file as byte array)
byte[] oleData;
try
{
string sampleFilePath = "sample.xlsx";
oleData = File.ReadAllBytes(sampleFilePath);
}
catch (Exception ex)
{
Console.WriteLine($"Error reading sample file: {ex.Message}");
return;
}
try
{
// Call the Add method with parameters: (upperLeftRow, upperLeftColumn, height, width, imageData)
int oleIndex = worksheet.OleObjects.Add(5, 2, 200, 300, oleData);
Console.WriteLine($"OLE object added successfully at index: {oleIndex}");
Console.WriteLine($"Position: Row 5, Column 2");
Console.WriteLine($"Size: 200px height, 300px width");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("OleObjectAddDemo.xlsx");
}
}
}
```
### See Also
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
## Add(int, int, int, int, byte[], string) {#add_1}
Adds a linked OleObject to the collection.
```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int height, int width, byte[] imageData,
string linkedFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| height | Int32 | Height of oleObject, in unit of pixel. |
| width | Int32 | Width of oleObject, in unit of pixel. |
| imageData | Byte[] | Image of ole object as byte array. |
| linkedFile | String |  |
### Return Value
[`OleObject`](../../oleobject/) object index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare OLE object data
int upperLeftRow = 1;
int upperLeftColumn = 1;
int height = 200;
int width = 200;
byte[] imageData = File.ReadAllBytes("sample.ole");
string linkedFile = "sample.xlsx";
try
{
// Call the Add method with the specific parameter types
int index = worksheet.OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData, linkedFile);
Console.WriteLine($"OLE object added at index: {index}");
Console.WriteLine($"Total OLE objects in worksheet: {worksheet.OleObjects.Count}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("OleObjectAddDemo.xlsx");
}
}
}
```
### See Also
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
