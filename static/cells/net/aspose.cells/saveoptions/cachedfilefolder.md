##SaveOptions.CachedFileFolder
SaveOptions property. The folder for temporary files that may be used as data cache
## SaveOptions.CachedFileFolder property
The folder for temporary files that may be used as data cache.
```csharp
public string CachedFileFolder { get; set; }
```
### Remarks
If the folder has not been specified, the default value for it is [`GetCacheFolder`](../../cellshelper/getcachefolder/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyCachedFileFolderDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test cached file folder");
// Set save options with cached file folder
SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
saveOptions.CachedFileFolder = "TempCache"; // Specify cache folder
// Save the workbook
workbook.Save("output.xml", saveOptions);
Console.WriteLine("File saved with cached file folder option.");
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
