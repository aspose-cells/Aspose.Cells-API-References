##EbookSaveOptions.EbookSaveOptions
EbookSaveOptions constructor. Creates options for saving ebook file
## EbookSaveOptions() {#constructor}
Creates options for saving ebook file.
```csharp
public EbookSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class EbookSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample content
worksheet.Cells["A1"].PutValue("Ebook Test");
worksheet.Cells["A2"].PutValue("This is a test for EbookSaveOptions");
// Create EbookSaveOptions using constructor
EbookSaveOptions saveOptions = new EbookSaveOptions();
// Save the workbook with EbookSaveOptions (automatically saves as EPUB)
workbook.Save("output.epub", saveOptions);
Console.WriteLine("Ebook saved successfully with EbookSaveOptions constructor.");
}
}
}
```
### See Also
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
## EbookSaveOptions(SaveFormat) {#constructor_1}
Creates options for saving ebook file.
```csharp
public EbookSaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Epub or Azw3. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Saving;
using System;
public class EbookSaveOptionsMethodCtorWithSaveFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to worksheet
worksheet.Cells["A1"].PutValue("Sample Ebook Content");
try
{
// Call the #ctor method with SaveFormat parameter
EbookSaveOptions saveOptions = new EbookSaveOptions(SaveFormat.Epub);
// Set additional properties if needed
saveOptions.Encoding = System.Text.Encoding.UTF8;
Console.WriteLine("EbookSaveOptions constructor executed successfully with SaveFormat.Epub");
// Save the workbook with the created options
workbook.Save("EbookSaveOptionsDemo.epub", saveOptions);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing EbookSaveOptions constructor: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
