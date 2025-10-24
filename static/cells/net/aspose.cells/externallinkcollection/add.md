##ExternalLinkCollection.Add
ExternalLinkCollection method. Adds an external link
## Add(string, string[]) {#add_1}
Adds an external link.
```csharp
public int Add(string fileName, string[] sheetNames)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The external file name. |
| sheetNames | String[] | All sheet names of the external file. |
### Return Value
The position of the external name in this list.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ExternalLinkCollectionMethodAddWithStringStringArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the external links collection
ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
// Prepare parameters for Add method
string fileName = "ExternalWorkbook.xlsx";
string[] sheetNames = new string[] { "Sheet1", "Sheet2" };
try
{
// Call the Add method with (String, String[]) parameters
int index = externalLinks.Add(fileName, sheetNames);
Console.WriteLine($"External link added at index: {index}");
Console.WriteLine($"Total external links: {externalLinks.Count}");
// Display added external link information
ExternalLink link = externalLinks[index];
Console.WriteLine($"External link file: {link.DataSource}");
Console.WriteLine("Referenced sheets:");
foreach (string sheet in sheetNames)
{
Console.WriteLine($"- {sheet}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the workbook
workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
}
}
}
```
### See Also
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(DirectoryType, string, string[]) {#add}
Add an external link .
```csharp
public int Add(DirectoryType directoryType, string fileName, string[] sheetNames)
```
| Parameter | Type | Description |
| --- | --- | --- |
| directoryType | DirectoryType | The directory type of the file name. |
| fileName | String | the file name. |
| sheetNames | String[] | All sheet names of the external file. |
### Return Value
The position of the external name in this list.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ExternalLinkCollectionMethodAddWithDirectoryTypeStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the external links collection
ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
// Prepare parameters for Add method
DirectoryType directoryType = DirectoryType.Volume; // Changed from Directory to Volume
string fileName = "ExternalWorkbook.xlsx";
string[] sheetNames = new string[] { "Sheet1", "Sheet2" };
try
{
// Call the Add method with (DirectoryType, String, String[]) parameters
int index = externalLinks.Add(directoryType, fileName, sheetNames);
Console.WriteLine($"External link added at index: {index}");
Console.WriteLine($"Total external links: {externalLinks.Count}");
// Display information about the added external link
ExternalLink link = externalLinks[index];
Console.WriteLine($"External link references: {link.DataSource}");
foreach (string sheet in sheetNames) // Changed from link.SheetNames to sheetNames
{
Console.WriteLine($" - References sheet: {sheet}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the workbook
workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
}
}
}
```
### See Also
* enum [DirectoryType](../../directorytype/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
