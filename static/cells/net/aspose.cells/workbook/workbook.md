##Workbook.Workbook
Workbook constructor. Initializes a new instance of the Workbook class
## Workbook() {#constructor}
Initializes a new instance of the [`Workbook`](../) class.
```csharp
public Workbook()
```
### Remarks
The default file format type is Xlsx. If you want to create other types of files, please use Workbook(FileFormatType).
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCtorDemo
{
public static void Run()
{
// Create a new workbook using the constructor
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["B1"].PutValue("World");
// Save the workbook
workbook.Save("WorkbookCtorDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Workbook created and saved successfully.");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Workbook(FileFormatType) {#constructor_1}
Initializes a new instance of the [`Workbook`](../) class.
```csharp
public Workbook(FileFormatType fileFormatType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fileFormatType | FileFormatType | The new file format. |
### Remarks
The default file format type is Excel97To2003.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCtorWithFileFormatTypeDemo
{
public static void Run()
{
// Create a new workbook with XLSX file format
Workbook workbook = new Workbook(FileFormatType.Xlsx);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Put some data in cell A1
worksheet.Cells["A1"].PutValue("Hello World!");
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Workbook(string) {#constructor_4}
Initializes a new instance of the [`Workbook`](../) class and open a file.
```csharp
public Workbook(string file)
```
| Parameter | Type | Description |
| --- | --- | --- |
| file | String | The file name. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCtorWithStringDemo
{
public static void Run()
{
// The path to the documents directory.
string dataDir = "Your Document Directory";
// Create a Workbook from an existing Excel file
Workbook workbook = new Workbook(dataDir + "example.xlsx");
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Display some worksheet information
Console.WriteLine("Worksheet Name: " + worksheet.Name);
Console.WriteLine("Number of Cells: " + worksheet.Cells.Count);
// Save the workbook in MHTML format
workbook.Save(dataDir + "output.mht", SaveFormat.MHtml);
// Create another Workbook from the saved MHTML file
Workbook workbook2 = new Workbook(dataDir + "output.mht");
Console.WriteLine("Number of Worksheets in MHTML: " + workbook2.Worksheets.Count);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Workbook(Stream) {#constructor_2}
Initializes a new instance of the [`Workbook`](../) class and open a stream.
```csharp
public Workbook(Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Workbook(string, LoadOptions) {#constructor_5}
Initializes a new instance of the [`Workbook`](../) class and open a file.
```csharp
public Workbook(string file, LoadOptions loadOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| file | String | The file name. |
| loadOptions | LoadOptions | The load options |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCtorWithStringLoadOptionsDemo
{
public static void Run()
{
// Create load options without LightCellsDataHandler
LoadOptions loadOptions = new LoadOptions();
// Initialize workbook with file path and load options
Workbook workbook = new Workbook("sample.xlsx", loadOptions);
// Demonstrate workbook is loaded by accessing worksheet count
Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
}
}
}
```
### See Also
* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Workbook(Stream, LoadOptions) {#constructor_3}
Initializes a new instance of the [`Workbook`](../) class and open stream.
```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| loadOptions | LoadOptions | The load options |
### See Also
* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
