##Class FolderFontSource
Aspose.Cells.FolderFontSource class. Represents the folder that contains TrueType font files
## FolderFontSource class
Represents the folder that contains TrueType font files.
```csharp
public class FolderFontSource : FontSourceBase
```
## Constructors
| Name | Description |
| --- | --- |
| [FolderFontSource](folderfontsource/)(string, bool) | Ctor. |
## Properties
| Name | Description |
| --- | --- |
| [FolderPath](../../aspose.cells/folderfontsource/folderpath/) { get; } | Path to fonts folder. |
| [ScanSubFolders](../../aspose.cells/folderfontsource/scansubfolders/) { get; } | Determines whether or not to scan the subfolders. |
| override [Type](../../aspose.cells/folderfontsource/type/) { get; } | Returns the type of the font source. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FolderFontSourceDemo
{
public static void FolderFontSourceExample()
{
// Create an instance of FolderFontSource
string folderPath = @"C:\Fonts";
bool scanSubfolders = true;
FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);
// Accessing properties
Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
Console.WriteLine("Font Source Type: " + folderFontSource.Type);
// Create a workbook and set the font sources
Workbook workbook = new Workbook();
FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
// Save the workbook
workbook.Save("FolderFontSourceExample.xlsx");
workbook.Save("FolderFontSourceExample.pdf");
return;
}
}
}
```
### See Also
* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
