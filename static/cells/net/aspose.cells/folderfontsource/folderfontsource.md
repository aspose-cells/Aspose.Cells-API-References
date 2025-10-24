##FolderFontSource.FolderFontSource
FolderFontSource constructor. Ctor
## FolderFontSource constructor
Ctor.
```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| folderPath | String | path to fonts folder |
| scanSubfolders | Boolean | Determines whether or not to scan subfolders. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FolderFontSourceMethodCtorWithStringBooleanDemo
{
public static void Run()
{
string folderPath = @"C:\Fonts";
bool scanSubfolders = true;
FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);
Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
Workbook workbook = new Workbook();
FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
workbook.Save("FolderFontSourceExample.xlsx");
}
}
}
```
### See Also
* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
