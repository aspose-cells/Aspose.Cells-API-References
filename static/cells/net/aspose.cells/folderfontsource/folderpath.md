##FolderFontSource.FolderPath
FolderFontSource property. Path to fonts folder
## FolderFontSource.FolderPath property
Path to fonts folder.
```csharp
public string FolderPath { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FolderFontSourcePropertyFolderPathDemo
{
public static void Run()
{
// Create a folder font source
string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
bool scanSubfolders = true;
FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);
// Demonstrate FolderPath property usage
Console.WriteLine("Font folder path: " + folderFontSource.FolderPath);
Console.WriteLine("Scan subfolders: " + folderFontSource.ScanSubFolders);
// Create workbook with the font source
Workbook workbook = new Workbook();
FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
// Simple demonstration - add text that might use custom fonts
workbook.Worksheets[0].Cells["A1"].PutValue("Font Source Demo");
// Save outputs
workbook.Save("FolderFontSourceDemo.xlsx");
}
}
}
```
### See Also
* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
