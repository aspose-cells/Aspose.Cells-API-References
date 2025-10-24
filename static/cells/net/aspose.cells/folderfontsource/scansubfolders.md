##FolderFontSource.ScanSubFolders
FolderFontSource property. Determines whether or not to scan the subfolders
## FolderFontSource.ScanSubFolders property
Determines whether or not to scan the subfolders.
```csharp
public bool ScanSubFolders { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FolderFontSourcePropertyScanSubFoldersDemo
{
public static void Run()
{
// Create a folder font source with subfolder scanning enabled
string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
bool scanSubfolders = true;
FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);
// Display font source properties
Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
// Create a workbook and set the font source
Workbook workbook = new Workbook();
FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
// Demonstrate usage by setting some text
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Text with fonts from folder source");
// Save the workbook
workbook.Save("FolderFontSourceDemo.xlsx");
}
}
}
```
### See Also
* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
