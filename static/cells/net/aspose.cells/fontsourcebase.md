##Class FontSourceBase
Aspose.Cells.FontSourceBase class. This is an abstract base class for the classes that allow the user to specify various font sources
## FontSourceBase class
This is an abstract base class for the classes that allow the user to specify various font sources
```csharp
public abstract class FontSourceBase
```
## Properties
| Name | Description |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | Returns the type of the font source. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassFontSourceBaseDemo
{
public static void Run()
{
// Create a folder font source
string fontFolder = @"C:\Windows\Fonts";
FolderFontSource folderSource = new FolderFontSource(fontFolder, true);
// Display font source properties
Console.WriteLine($"Font folder: {folderSource.FolderPath}");
Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
Console.WriteLine($"Source type: {folderSource.Type}");
// Create workbook and set font source
Workbook workbook = new Workbook();
FontConfigs.SetFontSources(new FontSourceBase[] { folderSource });
// Save with custom fonts
workbook.Save("OutputWithCustomFonts.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
